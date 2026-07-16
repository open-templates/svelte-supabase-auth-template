---
type: Reference
title: Key files
description: Source map for auth, API, layout, and pages.
tags: [reference, files]
timestamp: 2026-07-15T00:00:00Z
---

# Key files

| Path | Role |
|------|------|
| `src/lib/auth.ts` | Supabase auth stores, methods, `initAuth` |
| `src/routes.ts` | `svelte-spa-router` map + `wrap` conditions |
| `src/lib/api.ts` | Shared `apiFetch` with JWT + retry |
| `src/components/AppHeader.svelte` | Global header + health dot |
| `src/routes/Home.svelte` | Authenticated landing page |
