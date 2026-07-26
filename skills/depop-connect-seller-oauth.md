---
name: Connect a Depop seller via OAuth
description: Exchange an authorization code (PKCE) for tokens and read the connected shop.
api: openapi/depop-selling-openapi-original.yml
operations: [exchangeToken, getSellerDetails]
---

# Connect a Depop seller via OAuth

Let a Depop seller authorize your application to act on their shop.

## Flow (OAuth 2.0 Authorization Code + PKCE)
1. Generate a PKCE `code_verifier` and its S256 `code_challenge`.
2. Redirect the seller to Depop's authorization page requesting the scopes you
   need (`products_read`, `products_write`, `orders_read`, `orders_write`,
   `offers_read`, `offers_write`, `shop_read`). The seller logs in and approves.
3. **Exchange the code** — `POST /api/v1/oauth2/access-token/` (`exchangeToken`)
   with `grant_type=authorization_code`, the `code`, and the `code_verifier`
   (`application/x-www-form-urlencoded`, per RFC 6749 + RFC 7636). You receive a
   short-lived access token and a long-lived refresh token.
4. **Confirm** — `GET /api/v1/shop/` (`getSellerDetails`) to read the connected
   seller's id, username and country.
5. **Refresh** — when the access token expires, call `exchangeToken` again with
   `grant_type=refresh_token`.

## Rules
- Store the refresh token securely; never expose tokens client-side.
- A `403 insufficient_scope` means the token lacks a scope the endpoint needs.
- See authentication/depop-authentication.yml and scopes/depop-scopes.yml.
