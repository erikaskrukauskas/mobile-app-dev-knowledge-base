---
title: A notification opens the screen that holds the state
tags: [practices, navigation, screen, state, mobile]
status: tested
updated: 2026-10-19
---

# A notification opens the screen that holds the state

A notification is a hint that something changed. The state lives in the app.

## Rule

Tapping the notification opens the screen that shows the current state. The notification's text is not the record. If the state is already gone, open the fallback from [A deep link has a fallback screen](19-deep-link-fallback.md).

## Specify

- What the notification claims.
- The screen it opens.
- The fallback when the underlying state is gone.

## Check

Tap a notification for an item that exists, and for one that was deleted. The first opens the item. The second opens the fallback. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [About deep links](https://developer.android.com/training/app-links). The page supports this rule: Deep links bring users directly into app content from notifications, among other places.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Do not start a new flow in the background](14-no-new-flow-from-background.md)
- [A deep link has a fallback screen](19-deep-link-fallback.md)
