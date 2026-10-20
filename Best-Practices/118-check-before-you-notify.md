---
title: Check that alerts are allowed before you send one
tags: [practices, screen, permissions, mobile]
status: tested
updated: 2026-10-19
---

# Check that alerts are allowed before you send one

A grant from last month may have been turned off in system settings.

## Rule

Before posting an alert, check that alerts are enabled. If they are not, leave the state in the app and follow the denial path. Do not queue a stack of alerts that will be dropped.

## Specify

- Where the check runs.
- What is not posted when alerts are off.
- Where the same news appears inside the app.

## Check

Turn alerts off in settings, trigger the event, and confirm no system alert appears and the in-app screen still shows the state. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: Before your app sends a notification, confirm whether the user has enabled notifications for your app.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Notification permission is its own decision](86-notification-permission-is-separate.md)
- [A notification opens the screen that holds the state](85-notification-opens-the-state.md)
