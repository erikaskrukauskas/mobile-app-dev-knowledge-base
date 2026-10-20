---
title: Dismissing an alert prompt is not allow or deny
tags: [practices, permissions, screen, mobile]
status: tested
updated: 2026-10-19
---

# Dismissing an alert prompt is not allow or deny

Swiping a permission dialog away is not the same as refusing, and it is not the same as agreeing.

## Rule

If the person dismisses the prompt without choosing, leave the previous state in place and do not treat it as a permanent denial or as a grant. The next meaningful action can ask again.

## Specify

- The state before the prompt.
- The state after a swipe-away.
- The state after allow and after deny.

## Check

Open the prompt and dismiss it without choosing. Alerts stay in the prior state. Deny in a second run and the denial path appears. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: If the user swipes away from the dialog without choosing allow or don't allow, the state of the notification permission doesn't change.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A denied permission is explained in text](42-permission-failure-is-text.md)
