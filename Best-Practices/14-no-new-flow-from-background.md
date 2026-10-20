---
title: Do not start a new flow in the background
tags: [practices, lifecycle, navigation, mobile]
status: tested
updated: 2026-10-19
---

# Do not start a new flow in the background

A process that is not in front of the person should not open a new screen over whatever they are doing now.

## Rule

Background work may update state and, when allowed, post a notification. It does not push a new screen until the person opens the app or the notification.

## Specify

- Which events may arrive while the app is backgrounded.
- What they update.
- What the person sees if they are in another app.

## Check

Trigger the event while the app is backgrounded. No new screen appears until the person opens the app or the notification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [The activity lifecycle](https://developer.android.com/guide/components/activities/activity-lifecycle). The page supports this rule: With a few exceptions, apps are restricted from starting activities when running in the background.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A notification opens the screen that holds the state](85-notification-opens-the-state.md)
