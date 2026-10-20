---
title: Notification permission is its own decision
tags: [practices, permissions, screen, mobile]
status: tested
updated: 2026-10-19
---

# Notification permission is its own decision

Being allowed to run the app is not the same as being allowed to interrupt the person.

## Rule

Ask for notification permission when the person opts into an alert, not at first launch. If they refuse, the in-app screen still shows the state.

## Specify

- The alert they opted into.
- When the prompt appears.
- What still works after a refusal.

## Check

Refuse notifications and complete the task in the app. The state is on screen. The system notification is absent. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: Request permissions as late as possible, and only the permissions the action needs. An alert the person has not asked for is not yet that action.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Ask for a permission at the action](48-ask-at-the-action.md)
- [A notification opens the screen that holds the state](85-notification-opens-the-state.md)
