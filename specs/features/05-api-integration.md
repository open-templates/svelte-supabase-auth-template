---
type: Feature
title: API integration
description: health.ts and me.ts modules calling the paired worker.
tags: [api, health, jwt]
timestamp: 2026-07-15T00:00:00Z
---

# Modules (`src/api/`)

| Module | Endpoint | Auth | Used by |
|--------|----------|------|---------|
| `health.ts` | `GET /health` | No | `useApiHealth` → `AppHeader` |
| `me.ts` | `GET /me` | Bearer JWT | `HomePage` |

Base URL: `import.meta.env.VITE_API_BASE_URL` (default `http://localhost:8787`).

See [.agents/skills/shared/auth/jwt-api-passthrough.md](../../.agents/skills/shared/auth/jwt-api-passthrough.md).
