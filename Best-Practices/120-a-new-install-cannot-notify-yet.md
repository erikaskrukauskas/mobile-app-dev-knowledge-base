---
title: A new install cannot notify until the person allows it
tags: [practices, permissions, screen, mobile]
status: tested
updated: 2026-10-19
---

# A new install cannot notify until the person allows it

Installing the app is not permission to interrupt them.

## Rule

Until they grant alerts, do not post them. The in-app screens still work. Ask later, at the action that wants an alert, not as the first thing the new install does.

## Specify

- What works with alerts off.
- The action that may ask.
- What a restore does if a previous install had already allowed alerts: check, do not ask again blindly.

## Check

Install fresh and use the app. No alert appears and no prompt appears before they try the feature that wants one. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: If a user installs your app on a device that runs Android 13 or higher, your app's notifications are off by default. Your app must wait to send notifications until the user grants the permission. Wait to show the prompt until they have had a chance to learn the app.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Notification permission is its own decision](86-notification-permission-is-separate.md)
- [The first screen does not ask for sensitive access](102-first-screen-asks-for-nothing-sensitive.md)
