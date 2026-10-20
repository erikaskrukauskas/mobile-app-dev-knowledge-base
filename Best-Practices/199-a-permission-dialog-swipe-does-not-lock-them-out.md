---
title: A dismissed prompt does not lock the feature
tags: [practices, permissions, screen, mobile]
status: tested
updated: 2026-10-19
---

# A dismissed prompt does not lock the feature

Treating a swipe-away as a permanent denial sends them to settings for a choice they never made.

## Rule

Only a real denial uses the permanent-denial path. A dismissed prompt leaves the feature available to ask again on the next attempt.

## Specify

- Dismiss.
- Deny.
- Allow.

## Check

Dismiss the prompt, trigger the action again, and confirm the prompt can return. Deny in another run and the denial path appears. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: Swiping the notification-permission dialog away does not change the permission state. Don't allow does.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A permanent denial has a way forward](50-permanent-denial-path.md)
- [Dismissing an alert prompt is not allow or deny](119-dismissing-the-prompt-is-not-a-choice.md)
