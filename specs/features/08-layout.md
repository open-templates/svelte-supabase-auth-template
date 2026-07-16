---
type: Feature
title: Layout
description: ThemeProvider, Router, AuthProvider, and AppLayout hierarchy.
tags: [ui, architecture]
timestamp: 2026-07-15T00:00:00Z
---

# Hierarchy

```text
App
└── ThemeProvider
    └── Router
        └── AuthProvider
            └── AppLayout
                ├── AppHeader   (health + sign out when logged in)
                └── Outlet      (HomePage or auth pages)
```
