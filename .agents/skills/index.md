---
okf_version: "0.1"
---

# svelte-supabase-auth-template skills

Module guides for recreating auth, API, and layout patterns. Shared concepts are synced from the workspace `.agents/skills/` bundle.

## Shared (synced)

* [auth/](shared/auth/) - Supabase session, JWT passthrough, route guards
* [supabase/](shared/supabase/) - OAuth setup, worker client helpers

## Local modules

* [api-fetch](modules/api-fetch.md) - `apiFetch` with Bearer token and 401 retry
* [app-header-health](modules/app-header-health.md) - health polling hook and header UI

## Agent skills

Framework guidance: [README.md](README.md)

## Specs

Feature contracts: [index.md](../../index.md)
