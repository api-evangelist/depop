---
name: List a product on Depop
description: Create or update a Depop listing keyed on your own SKU, verify it, and mark it sold.
api: openapi/depop-selling-openapi-original.yml
operations: [createOrUpdateProduct, getProductBySku, markProductAsSold]
---

# List a product on Depop

Use the Depop Selling API to publish and manage a listing.

## Auth
Send `Authorization: Bearer <token>` on every request — a per-shop API key
(prefix `pak_`) or an OAuth 2.0 access token holding `products_write` (and
`offers_write` if you set `auto_send_offer_price` / `auto_negotiate_offer_price`).

## Steps
1. **Create or update the listing** — `PUT /api/v1/products/by-sku/{sku}/`
   (`createOrUpdateProduct`). Choose a unique, non-reusable `sku`. If the SKU is
   new a listing is created; if it exists it is updated. This call is idempotent
   on the SKU, so retries converge rather than duplicating.
2. **Verify** — `GET /api/v1/products/by-sku/{sku}/` (`getProductBySku`) and
   confirm the returned product state.
3. **Mark as sold** (when sold outside the API) —
   `POST /api/v1/products/by-sku/{sku}/mark-as-sold/` (`markProductAsSold`).

## Rules
- Respect rate limits: 20 requests/second for create-or-update, 100 rps
  cumulative elsewhere; back off on `429`.
- Errors come as `{ id, errors: [{ code, message }] }`. Handle `422`
  (`missing_attribute`/validation) and `409` (product has active offers).
- See conventions/depop-conventions.yml and errors/depop-problem-types.yml.
