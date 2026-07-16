---
type: Playbook
title: Extension guidelines
description: Safe patterns for adding routes, API modules, and documentation.
tags: [extension, maintainer]
timestamp: 2026-07-15T00:00:00Z
---

# Guidelines

1. Add new API modules under `src/api/` using `apiFetch`.
2. Register routes in `src/App.tsx` inside `AppLayout` with appropriate `AuthGuard`.
3. Add a numbered concept under `specs/features/` and link it from [index.md](../../index.md).
4. Add or update `.agents/skills/modules/` when introducing a reusable pattern.
5. Do not put service role keys or secrets in `VITE_*` variables.

When adding a backend route, document both sides in each repo's `specs/` bundle.
