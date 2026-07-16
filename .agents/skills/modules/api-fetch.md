---
type: Playbook
title: apiFetch
description: Recreate the shared API client with JWT attachment and session refresh.
tags: [api, jwt, react]
timestamp: 2026-07-15T00:00:00Z
resource: src/api/api.ts
---

# Pattern

1. `const baseUrl = import.meta.env.VITE_API_BASE_URL`
2. Read `localStorage.getItem('x-auth-token')` for `Authorization`
3. On `401`, `await supabase.auth.refreshSession()`, update token, retry once
4. Parse JSON; surface `{ data, error }` to callers

# Used by

`src/api/health.ts`, `src/api/me.ts`

# See also

* [shared/auth/jwt-api-passthrough.md](../shared/auth/jwt-api-passthrough.md)
* [specs/features/05-api-integration.md](../../specs/features/05-api-integration.md)
