---
title: The metered warning comes before the bytes move
tags: [practices, screen, offline, mobile]
status: tested
updated: 2026-10-19
---

# The metered warning comes before the bytes move

Asking after a large upload has started does not give them the choice.

## Rule

Check the metered state before starting the large transfer. The confirmation is the start, not an apology.

## Specify

- The check.
- The confirmation.
- The small requests that do not ask.

## Check

Begin a large transfer on a metered network and confirm nothing is sent before they agree. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: You can tell that a network is metered from its capabilities, and you can schedule large work for an unmetered network instead of starting it immediately.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A large transfer respects a metered network](128-large-transfer-respects-a-metered-network.md)
