---
title: Alerts and the in-app screen are allowed to diverge
tags: [practices, screen, permissions, mobile]
status: tested
updated: 2026-10-19
---

# Alerts and the in-app screen are allowed to diverge

Turning off alerts is not deleting the data.

## Rule

The in-app screen shows the state whether or not alerts are allowed. Turning alerts off does not clear the unread state. Turning them on does not invent new items.

## Specify

- What the screen shows with alerts off.
- What an alert would have said.
- The unread state, which is independent.

## Check

Turn alerts off with unread items present. The items are still in the app. The badge still matches them. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: A denial blocks notification channels. It does not describe deleting the underlying user-visible state inside the app.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A badge matches the unread state](87-badge-matches-unread-state.md)
- [Notification permission is its own decision](86-notification-permission-is-separate.md)
