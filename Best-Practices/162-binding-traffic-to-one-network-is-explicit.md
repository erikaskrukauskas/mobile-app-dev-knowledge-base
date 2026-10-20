---
title: Binding traffic to one network is explicit
tags: [practices, security, offline, mobile]
status: tested
updated: 2026-10-19
---

# Binding traffic to one network is explicit

Forcing all traffic onto one network can need a separate permission and can surprise the person when that network drops.

## Rule

Use the system's default network unless the task truly must use a named one. If you bind, say so, request only that capability, and handle the moment that network disappears.

## Specify

- Which calls bind.
- Why.
- The screen when that network goes away.

## Check

Drop the bound network during a transfer. The screen explains it. Ordinary screens never needed the bind. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: Binding to a background network requires a specific permission. A Network object stops being usable when the network disconnects.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Request the smallest permission](44-smallest-permission.md)
