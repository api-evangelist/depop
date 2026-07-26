---
name: Fulfill and refund a Depop order
description: Poll orders, mark a parcel shipped with tracking, and issue a refund.
api: openapi/depop-selling-openapi-original.yml
operations: [getAllOrders, getOrderByPurchaseId, markOrderAsShipped, refundOrder]
---

# Fulfill and refund a Depop order

## Auth
`Authorization: Bearer <token>` with `orders_read` (read) and `orders_write`
(ship/refund) scopes. Prefer webhooks over polling: subscribe to `newOrder` and
`orderRefunded` (see asyncapi/depop-webhooks-asyncapi.yml).

## Steps
1. **Discover orders** — `GET /api/v1/orders/` (`getAllOrders`), or react to a
   `newOrder` webhook carrying the `purchase_id`.
2. **Read one order** — `GET /api/v1/orders/{purchase_id}/`
   (`getOrderByPurchaseId`) to get line items, buyer address and parcels.
3. **Mark shipped** — `POST /api/v1/orders/{purchase_id}/parcels/{parcel_id}/mark-as-shipped/`
   (`markOrderAsShipped`), supplying tracking information.
4. **Refund if needed** — `POST /api/v1/orders/{purchase_id}/refund/`
   (`refundOrder`); the response breaks the refund down to buyer and seller.

## Rules
- Handle `404` (order not found) and `422` (validation) on the error envelope
  `{ id, errors[] }`. Back off on `429`.
