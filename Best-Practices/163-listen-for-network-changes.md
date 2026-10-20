---
title: Listen for network changes instead of polling
tags: [practices, offline, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Listen for network changes instead of polling

Polling connectivity keeps the device awake and still misses fast changes.

## Rule

Subscribe to the connectivity changes the screen cares about, update when they happen, and stop listening when the screen is gone.

## Specify

- The changes that matter.
- What the screen does on each.
- When the listener stops.

## Check

Toggle the network while the screen is open. The screen updates. Leave the screen and confirm the listener is not still running for it. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: Register a callback to react to connectivity changes without expensive polling that might miss fast updates. Synchronous checks do not update the UI later.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Release work when the app is not visible](12-release-work-when-backgrounded.md)
- [A connected network is not a successful response](129-a-network-object-is-not-success.md)
