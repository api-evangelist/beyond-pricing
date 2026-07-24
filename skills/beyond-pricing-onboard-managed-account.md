---
name: Onboard a Beyond user and connect a managed account
description: Create a Beyond user, connect their PMS/OTA managed account, refresh it, and confirm their listings synced.
api: openapi/beyond-pricing-openapi-original.yml
operations: [create_user, create_account, refresh_account, list_listings]
---

# Onboard a Beyond user and connect a managed account

Use this to bring a new customer onto the Beyond platform through the Partners API.

## Auth
Use an OAuth2 **client-credentials** token (partner, confidential client). Mint it at
`POST https://developers.beyondpricing.com/o/token/` with `grant_type=client_credentials`.
Creating a user needs the app-level `user:write` scope (no `user_id`). Connecting the
account and listing operations need a **user-scoped** token (include `user_id`) with
`accounts:read` and `listings:read`. Send `Authorization: Bearer <token>`; tokens expire
after 1 hour. All bodies use JSON:API (`application/vnd.api+json`).

## Steps
1. **create_user** — `POST /api/v1/users/` with the customer's details. Save the returned
   user `id`. (If it returns `409 Conflict`, the email already exists — look it up with
   list users `filter[email]=`.)
2. **create_account** — `POST /api/v1/users/{user_id}/accounts/` with the managed channel
   (PMS/OTA) credentials to connect. Requires a user-scoped token.
3. **refresh_account** — `POST /api/v1/users/{user_id}/accounts/{account_id}/refresh/` to
   trigger the listing sync. If it returns `409 Conflict`, a sync is already in progress —
   wait for the `account.refreshed` webhook (or poll) and do not re-fire.
4. **list_listings** — `GET /api/v1/listings/` (user-scoped token) to confirm the synced
   listings appeared. Page with `page[number]`/`page[size]` (max 100).

## Rules
- Prefer webhooks over polling: subscribe to `account.created` / `account.refreshed` to
  learn when the background sync finishes instead of looping on refresh.
- Honor `429` `Retry-After` and watch `X-RateLimit-Remaining`.
- Errors are JSON:API `errors[]` (`status`/`title`/`detail`/`source.pointer`) — see
  errors/beyond-pricing-problem-types.yml.
