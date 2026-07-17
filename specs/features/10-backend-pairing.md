---
type: Feature
title: Backend pairing
description: Contract with cf-hono-supabase-api-template for /health and /me.
tags: [pairing, api, hono]
timestamp: 2026-07-15T00:00:00Z
resource: https://github.com/open-templates/cf-hono-supabase-api-template
---

# Pairing

Requires a backend implementing the same `/health` and `/me` contracts:

- **Cloudflare:** `cf-hono-supabase-api-template` (or FastAPI/Rust worker variants; default dev `http://localhost:8787`)
- **Docker / VM:** [vm-php-supabase-api-template](https://github.com/open-templates/vm-php-supabase-api-template) (default dev `http://localhost:8080`)

| Frontend call | Backend route |
|---------------|---------------|
| Header health dot | `GET /health` (no auth) |
| Home profile card | `GET /me` (Bearer from `x-auth-token`) |

Backend OKF specs: [cf-hono-supabase-api-template](https://github.com/open-templates/cf-hono-supabase-api-template/blob/main/index.md) · [vm-php-supabase-api-template](https://github.com/open-templates/vm-php-supabase-api-template/blob/main/index.md).
