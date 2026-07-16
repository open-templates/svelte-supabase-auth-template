---
type: Feature
title: Auth providers
description: Google OAuth and email/password flows via Supabase Auth.
tags: [auth, supabase, oauth]
timestamp: 2026-07-15T00:00:00Z
---

# Providers

* **Google OAuth** — `loginWithGoogle` in `AuthContext` (`signInWithOAuth`)
* **Email/password** — sign up, sign in, recover password, reset password

OAuth is configured entirely in the Supabase dashboard (no Google client ID in frontend env vars). See [.agents/skills/shared/supabase/dashboard-oauth-setup.md](../../.agents/skills/shared/supabase/dashboard-oauth-setup.md).
