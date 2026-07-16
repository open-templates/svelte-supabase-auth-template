# svelte-supabase-auth-template — Agent Skills Index

Skills in `.agents/skills/` teach agents how this repository works and how to extend it safely.

## Project status (current template)

Minimal **Svelte 5 + Supabase Auth** SPA paired with **cf-hono-supabase-api-template** (or any auth-pack backend):

- **Auth:** Google OAuth + email/password (`src/lib/auth.ts`, auth routes)
- **API calls:** `GET /health` (header indicator), `GET /me` (home page) via `apiFetch`
- **Routes:** `/`, `/login`, `/signup`, `/recover-password`, `/reset-password` (`svelte-spa-router`)

Canonical OKF specs: [`index.md`](../../index.md) · OKF modules: [`.agents/skills/index.md`](index.md)

## OKF modules (local)

| Module | Use when |
|--------|----------|
| [api-fetch](modules/api-fetch.md) | `apiFetch` with Bearer token and 401 retry |
| [app-header-health](modules/app-header-health.md) | health polling hook and header UI |

Shared concepts (synced): [shared/auth/](shared/auth/) · [shared/supabase/](shared/supabase/)

## Agent read order

1. `INSTRUCTIONS.md` → `index.md` → this file → `shared/auth/`
