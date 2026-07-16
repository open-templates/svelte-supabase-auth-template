---
type: Feature
title: Auth routes
description: Guest-only and authenticated routes with AuthGuard.
tags: [auth, routing, svelte-spa-router]
timestamp: 2026-07-15T00:00:00Z
resource: src/routes.ts
---

# Routes

| Route | Guard | Component |
|-------|-------|-----------|
| `/login` | Guest only | `Login.svelte` |
| `/signup` | Guest only | `Signup.svelte` |
| `/recover-password` | Guest only | `RecoverPassword.svelte` |
| `/reset-password` | Authenticated | `ResetPassword.svelte` |
| `/` | Authenticated | `Home.svelte` |

Guests hitting `/` redirect to `/login`. Authenticated users on auth pages redirect to `/`.

See [.agents/skills/shared/auth/route-guards.md](../../.agents/skills/shared/auth/route-guards.md).
