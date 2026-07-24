---
name: Tune a listing's dynamic pricing
description: Read a listing and its calendar, then adjust its base price and min/max price floor/ceiling customizations.
api: openapi/beyond-pricing-openapi-original.yml
operations: [get_listing, list_listing_calendar, get_listing_base_price_customization, patch_listing_base_price_customization, patch_listing_min_max_prices_customization]
---

# Tune a listing's dynamic pricing

Use this to inspect and adjust the dynamic-pricing controls for a single listing.

## Auth
Use a **user-scoped** OAuth2 client-credentials token (include `user_id`) or a personal
access token (`bpat_...`). Reading needs `listings:read`; the calendar needs
`reservations:read`; writing customizations needs `listings:write`. Send
`Authorization: Bearer <token>`. JSON:API (`application/vnd.api+json`) throughout.

## Steps
1. **get_listing** — `GET /api/v1/listings/{listing_id}/` to confirm the listing and read
   its current pricing state.
2. **list_listing_calendar** — `GET /api/v1/listings/{listing_id}/calendar/` to see modeled
   per-date prices, pricing factors (with `amount`), and `effective-min-price` /
   `effective-max-price`. Requires `reservations:read`.
3. **get_listing_base_price_customization** — `GET
   /api/v1/listings/{listing_id}/customizations/base-price/` to read the current base-price override.
4. **patch_listing_base_price_customization** — `PATCH
   /api/v1/listings/{listing_id}/customizations/base-price/` to set a new base price.
5. **patch_listing_min_max_prices_customization** — `PATCH
   /api/v1/listings/{listing_id}/customizations/min-max-prices/` to set the price floor and
   ceiling that bound the dynamic engine.

## Rules
- There is **no** request `Idempotency-Key`; PATCHes are naturally idempotent (they set a
  value). Re-read after writing to confirm the effective values via the calendar.
- A `listing.base_price_changed` webhook fires when the effective base price changes —
  reconcile against it rather than assuming your PATCH is the only source of change.
- Honor `429` `Retry-After`; errors are JSON:API `errors[]`.
