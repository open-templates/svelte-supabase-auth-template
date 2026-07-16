---
okf_version: "0.1"
---

# svelte-supabase-auth-template

OKF knowledge bundle for the out-of-the-box template surface. Start here before extending routes or API modules.

## Documentation

* [README.md](README.md) - quick start and environment
* [INSTRUCTIONS.md](INSTRUCTIONS.md) - maintainer and adopter guide

## Features

* [01 — Purpose](specs/features/01-purpose.md) - template goals and pairing
* [02 — Auth providers](specs/features/02-auth-providers.md) - Google OAuth and email/password
* [03 — Auth session](specs/features/03-auth-session.md) - session storage and token refresh
* [04 — Auth routes](specs/features/04-auth-routes.md) - guest vs protected routes
* [05 — API integration](specs/features/05-api-integration.md) - health and `/me` modules
* [06 — Health indicator](specs/features/06-health-indicator.md) - header polling behavior
* [07 — Home page](specs/features/07-home-page.md) - authenticated landing and JWT debug
* [08 — Layout](specs/features/08-layout.md) - app shell hierarchy
* [09 — Key files](specs/features/09-key-files.md) - source map
* [10 — Backend pairing](specs/features/10-backend-pairing.md) - cf-hono-supabase-api-template contract
* [11 — Extension guidelines](specs/features/11-extension-guidelines.md) - how to add features safely

## Skills

* [.agents/skills/index.md](.agents/skills/index.md) — OKF modules + shared concepts
* [.agents/skills/README.md](.agents/skills/README.md) — Cursor `SKILL.md` catalog
* [.agents/skills/shared/](.agents/skills/shared/) — synced auth and Supabase skills

## History

* [specs/log.md](specs/log.md)
