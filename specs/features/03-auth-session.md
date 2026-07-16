---
type: Feature
title: Auth session
description: Client session storage, x-auth-token mirror, and 401 refresh retry.
tags: [auth, session, jwt]
timestamp: 2026-07-15T00:00:00Z
resource: src/auth/AuthContext.tsx
---

# Session storage

* Supabase session via `onAuthStateChange`
* Access token mirrored to `localStorage['x-auth-token']` for API `Authorization: Bearer` headers
* On `401`, `apiFetch` attempts `supabase.auth.refreshSession()` and retries once

See [.agents/skills/shared/auth/supabase-session-flow.md](../../.agents/skills/shared/auth/supabase-session-flow.md).
