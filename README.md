# Beyond Pricing

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Beyond (formerly Beyond Pricing) is a revenue management platform for short-term and vacation rental businesses. Its dynamic pricing engine automatically adjusts nightly rates against real-time market demand across Airbnb, Vrbo, Booking.com and dozens of property management systems, and the platform adds market insights, direct-booking sites (Signal), payment processing (Tally), an AI pricing assistant (Neyoba) and owner reporting. The Beyond Partners API is a Bearer-protected, JSON:API (v1.1) REST API for third-party integrations: partners authenticate with OAuth2 client credentials on a confidential client (optionally narrowed to a single user or credential), while individual users automate their own accounts with personal access tokens (bpat_...). The API exposes listings, pricing calendars, listing customizations, competitive sets, recommendations, managed channel accounts, users, and market insights, with signed Standard Webhooks for real-time events, transparent rate-limit headers, URL-path versioning and a published deprecation policy.

**Areas:** Company · Short-Term Rental · Vacation Rentals · Revenue Management · Dynamic Pricing · Hospitality · Property Management · Travel · Pricing · JSON:API

## Beyond Pricing on APIs.io

Everything profiled for Beyond Pricing is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/beyond-pricing/](https://apis.io/providers/beyond-pricing/)** — or go straight to one of the APIs or properties below.

### APIs (8)

- [Beyond Pricing Accounts API](https://apis.io/apis/beyond-pricing/beyond-pricing-accounts-api/) — The Accounts API from Beyond Pricing — 3 operation(s) for accounts.
- [Beyond Pricing Compsets API](https://apis.io/apis/beyond-pricing/beyond-pricing-compsets-api/) — The Compsets API from Beyond Pricing — 2 operation(s) for compsets.
- [Beyond Pricing Customizations API](https://apis.io/apis/beyond-pricing/beyond-pricing-customizations-api/) — The Customizations API from Beyond Pricing — 6 operation(s) for customizations.
- [Beyond Pricing Insights API](https://apis.io/apis/beyond-pricing/beyond-pricing-insights-api/) — The Insights API from Beyond Pricing — 1 operation(s) for insights.
- [Beyond Pricing Listings API](https://apis.io/apis/beyond-pricing/beyond-pricing-listings-api/) — The Listings API from Beyond Pricing — 6 operation(s) for listings.
- [Beyond Pricing Users API](https://apis.io/apis/beyond-pricing/beyond-pricing-users-api/) — The Users API from Beyond Pricing — 3 operation(s) for users.
- [Beyond Pricing Webhooks API](https://apis.io/apis/beyond-pricing/beyond-pricing-webhooks-api/) — The Webhooks API from Beyond Pricing — 0 operation(s) for webhooks.
- [Beyond Pricing O Auth2 API](https://apis.io/apis/beyond-pricing/beyond-pricing-oauth2-api/) — The OAuth2 API from Beyond Pricing — 1 operation(s) for oauth2.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Beyond Pricing Webhooks](https://apis.io/asyncapis/beyond-pricing/beyond-pricing-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [beyond-pricing](https://apis.io/servers/beyond-pricing/beyond-pricing/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Beyond Pricing Agentic Access](https://apis.io/agentic-access/beyond-pricing/beyond-pricing-agentic-access/)

#### Collections (7)

Postman and Open Collection request collections.

- [Beyond Pricing Public Accounts API](https://apis.io/collections/beyond-pricing/open-beyond-pricing-accounts-api/)
- [Beyond Pricing Public Accounts Compsets API](https://apis.io/collections/beyond-pricing/open-beyond-pricing-compsets-api/)
- [Beyond Pricing Public Accounts Customizations API](https://apis.io/collections/beyond-pricing/open-beyond-pricing-customizations-api/)
- [Beyond Pricing Public Accounts Insights API](https://apis.io/collections/beyond-pricing/open-beyond-pricing-insights-api/)
- [Beyond Pricing Public Accounts Listings API](https://apis.io/collections/beyond-pricing/open-beyond-pricing-listings-api/)
- [Beyond Pricing Public Accounts OAuth2 API](https://apis.io/collections/beyond-pricing/open-beyond-pricing-oauth2-api/)
- [Beyond Pricing Public Accounts Users API](https://apis.io/collections/beyond-pricing/open-beyond-pricing-users-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Beyond Pricing Openapi Overlay](https://apis.io/overlays/beyond-pricing/beyond-pricing-openapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Beyond Pricing Authentication](https://apis.io/security/beyond-pricing/beyond-pricing-authentication/)
- [Beyond Pricing Domain Security](https://apis.io/security/beyond-pricing/beyond-pricing-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Beyond Pricing Scopes](https://apis.io/scopes/beyond-pricing/beyond-pricing-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.beyondpricing.com)
- [Documentation](https://developers.beyondpricing.com/)
- [Getting started](https://developers.beyondpricing.com/getting-started/)
- [API reference](https://developers.beyondpricing.com/api/v1/docs/)
- [Pricing](https://www.beyondpricing.com/plans)
- [Sign up](https://v2.beyondpricing.com/create-account/pricing)
- [Support](https://support.beyondpricing.com/)
- [Changelog](https://developers.beyondpricing.com/release-notes/)
- [Blog](https://beyondpricing.com/blog)
- [Terms of service](https://www.beyondpricing.com/legal/terms-of-service-2025)
- [Privacy policy](https://www.beyondpricing.com/legal/privacy)

## API Evangelist rating

**Kin Score 47.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 55.8 |
| Contract governance | 4.5 |
| Operational transparency | 31.6 |
| Developer ergonomics | 58.9 |
| Access clarity | 38.2 |

**Agent readiness 47.1** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | served (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | paginated |
| Operation Distinctiveness | distinct |

**Regulatory alignment 34.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/beyond-pricing/](https://apis.io/providers/beyond-pricing/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Beyond Pricing: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/beyond-pricing/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
