---
title: Stop listening when the screen closes
tags: [practices, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Stop listening when the screen closes

A listener that outlives the screen keeps the device working and can update the wrong generation of the screen.

## Rule

Cancel the screen's network and sensor listeners in the same lifecycle moment the screen stops being visible, unless a named ongoing task still owns them.

## Specify

- The listeners.
- The moment they stop.
- The ongoing task that is allowed to keep one.

## Check

Open the screen, leave it, and confirm its listener is not still running. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: Callbacks exist so the app can react while it cares. Pair that with the lifecycle rule that work which is only meaningful on screen stops when the screen is gone.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Release work when the app is not visible](12-release-work-when-backgrounded.md)
- [Listen for network changes instead of polling](163-listen-for-network-changes.md)
