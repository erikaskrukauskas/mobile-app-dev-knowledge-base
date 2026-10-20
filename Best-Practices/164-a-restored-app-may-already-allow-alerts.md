---
title: A restored app may already allow alerts
tags: [practices, permissions, state, mobile]
status: tested
updated: 2026-10-19
---

# A restored app may already allow alerts

A backup from a phone where they allowed alerts can arrive on a new phone with that choice already made.

## Rule

Check the current grant. Do not show a blocking enable-alerts screen when alerts are already allowed, and do not assume a fresh install's off default after a restore.

## Specify

- The check on first launch.
- The screen when alerts are already allowed.
- The screen when they are not.

## Check

Restore a backup from an install that had alerts allowed. The first launch does not demand the prompt again. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: When an app is restored, the system can treat it as an existing app and grant the notification permission so it can keep sending notifications.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A restore can finish before the first launch](108-restore-before-first-launch.md)
- [A new install cannot notify until the person allows it](120-a-new-install-cannot-notify-yet.md)
