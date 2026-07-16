---
type: Feature
title: Health indicator
description: Header polls GET /health every 30 seconds on all pages.
tags: [api, health, ui]
timestamp: 2026-07-15T00:00:00Z
resource: src/layout/AppHeader.tsx
---

# Behavior

* Polls every **30 seconds**
* States: `checking` (yellow), `online` (green), `offline` (red)
* Visible on **all** pages (including login) so users always see API connectivity
