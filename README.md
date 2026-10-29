# depop

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

Depop is a peer-to-peer fashion marketplace where people buy, sell and discover secondhand and unique clothing. Its Selling API is an enterprise partner API that lets approved partners automate the seller experience on Depop: create and manage listings (by SKU, product id or slug), manage orders, mark parcels shipped, issue refunds, submit and automate offers, read seller and shipping details, and pull shop and product insights. The API is OpenAPI 3.1, secured with per-shop API keys and OAuth 2.0 (Authorization Code + PKCE) with granular scopes, documents rate limits, and emits webhooks for new orders, refunds and product likes. Access is by invitation via developers@depop.com. Depop is backed by Balderton Capital, Creandum, EQT Ventures and HV Capital and is owned by Etsy.

**Areas:** Company · Fashion · Marketplace · E-Commerce · Resale · Retail · Inventory · Order · Sustainability

## depop on APIs.io

Everything profiled for depop is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/depop/](https://apis.io/providers/depop/)** — or go straight to one of the APIs or properties below.

### APIs (13)

- [depop API status API](https://apis.io/apis/depop/depop-api-status-api/) — Service health and status endpoints
- [depop Authentication API](https://apis.io/apis/depop/depop-authentication-api/) — OAuth 2.0 authentication endpoints for partner integration
- [depop Docs API](https://apis.io/apis/depop/depop-docs-api/) — The Docs API from depop — 1 operation(s) for docs.
- [depop Insights API](https://apis.io/apis/depop/depop-insights-api/) — Shop and product insights
- [depop Orders API](https://apis.io/apis/depop/depop-orders-api/) — Order management and fulfillment operations
- [depop Pricing Inspiration API](https://apis.io/apis/depop/depop-pricing-inspiration-api/) — ML-powered price recommendations and pricing guidance
- [depop Products API](https://apis.io/apis/depop/depop-products-api/) — General product operations
- [depop Products - By Product ID API](https://apis.io/apis/depop/depop-products-by-product-id-api/) — Product operations using internal product ID identifiers
- [depop Products - By SKU API](https://apis.io/apis/depop/depop-products-by-sku-api/) — Product operations using SKU (Stock Keeping Unit) identifiers
- [depop Products - By Slug API](https://apis.io/apis/depop/depop-products-by-slug-api/) — Product operations using URL-friendly slug identifiers
- [depop Products - Legacy (Deprecated) API](https://apis.io/apis/depop/depop-products-legacy-deprecated-api/) — Deprecated product endpoints - use By SKU or By Product ID alternatives instead
- [depop Shop Management API](https://apis.io/apis/depop/depop-shop-management-api/) — Shop and seller information endpoints
- [depop Seller API](https://apis.io/apis/depop/depop-seller-api-api/) — The Seller API API from depop — 0 operation(s) for seller api.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (2)

Multi-step workflows that chain operations into a business task.

- [List a product and mark it sold](https://apis.io/arazzos/depop/depop-list-and-sell.arazzo/)
- [Order fulfillment](https://apis.io/arazzos/depop/depop-order-fulfillment.arazzo/)

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Depop Selling API — Webhooks](https://apis.io/asyncapis/depop/depop-webhooks-asyncapi/)

#### Event channels (1)

Individual events and webhooks the provider emits.

- [{partnerWebhookUrl}](https://apis.io/channels/depop/partnerwebhookurl/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [depop-selling](https://apis.io/servers/depop/depop-selling/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Depop Agentic Access](https://apis.io/agentic-access/depop/depop-agentic-access/)

#### Collections (12)

Postman and Open Collection request collections.

- [Seller API status API](https://apis.io/collections/depop/open-depop-api-status-api/)
- [Seller API status Authentication API](https://apis.io/collections/depop/open-depop-authentication-api/)
- [Seller API status Docs API](https://apis.io/collections/depop/open-depop-docs-api/)
- [Seller API status Insights API](https://apis.io/collections/depop/open-depop-insights-api/)
- [Seller API status Orders API](https://apis.io/collections/depop/open-depop-orders-api/)
- [Seller API status Pricing Inspiration API](https://apis.io/collections/depop/open-depop-pricing-inspiration-api/)
- [Seller API status Products API](https://apis.io/collections/depop/open-depop-products-api/)
- [Seller API status Products - By Product ID API](https://apis.io/collections/depop/open-depop-products-by-product-id-api/)
- [Seller API status Products - By SKU API](https://apis.io/collections/depop/open-depop-products-by-sku-api/)
- [Seller API status Products - By Slug API](https://apis.io/collections/depop/open-depop-products-by-slug-api/)
- [Seller API status Products - Legacy (Deprecated) API](https://apis.io/collections/depop/open-depop-products-legacy-deprecated-api/)
- [Seller API status Shop Management API](https://apis.io/collections/depop/open-depop-shop-management-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Depop Selling Overlay](https://apis.io/overlays/depop/depop-selling-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Depop Authentication](https://apis.io/security/depop/depop-authentication/)
- [Depop Domain Security](https://apis.io/security/depop/depop-domain-security/)
- [Depop Vulnerability Disclosure](https://apis.io/security/depop/depop-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Depop Scopes](https://apis.io/scopes/depop/depop-scopes/)

#### Rate limits (1)

Published request limits.

- [Depop Rate Limits](https://apis.io/rate-limits/depop/depop-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.depop.com/)
- [Documentation](https://partnerapi.depop.com/api-docs/)
- [Getting started](https://partnerapi.depop.com/api-docs/getting-started/your-first-listing/)
- [API reference](https://partnerapi.depop.com/api-docs/reference/)
- [Support](https://depophelp.zendesk.com/)
- [Blog](https://engineering.depop.com/)
- [Security](https://www.depop.com/.well-known/security.txt)
- [Terms of service](https://www.depop.com/terms/)
- [Privacy policy](https://www.depop.com/privacy/)
- [GitHub](https://github.com/depop)
- [Status](https://depopstatus.com/)

## API Evangelist rating

**Kin Score 58.0** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 62.9 |
| Contract governance | 4.5 |
| Operational transparency | 81.6 |
| Developer ergonomics | 66.1 |
| Access clarity | 21.1 |

**Agent readiness 41.6** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | verified |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 40.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/depop/](https://apis.io/providers/depop/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for depop: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/depop/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
