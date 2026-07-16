---
type: Feature
title: Backend pairing
description: Contract with cf-hono-supabase-api-template for /health and /me.
tags: [pairing, api, hono]
timestamp: 2026-07-15T00:00:00Z
resource: https://github.com/open-templates/cf-hono-supabase-api-template
---

# Pairing

Requires **cf-hono-supabase-api-template** (or any API implementing the same `/health` and `/me` contracts).

| Frontend call | Backend route |
|---------------|---------------|
| Header health dot | `GET /health` (no auth) |
| Home profile card | `GET /me` (Bearer from `x-auth-token`) |

Backend OKF spec: [cf-hono-supabase-api-template/index.md](https://github.com/open-templates/cf-hono-supabase-api-template/blob/main/index.md).
