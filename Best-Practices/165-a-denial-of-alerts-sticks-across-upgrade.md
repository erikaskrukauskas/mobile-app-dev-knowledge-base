---
title: A previous alert denial still holds after an upgrade
tags: [practices, permissions, mobile]
status: tested
updated: 2026-10-19
---

# A previous alert denial still holds after an upgrade

An operating-system upgrade should not quietly turn alerts back on after the person turned them off.

## Rule

If they had disabled alerts, keep treating alerts as off after an upgrade until they allow them. Check. Do not celebrate the upgrade with a new prompt as the first screen.

## Specify

- The check.
- The in-app path while alerts stay off.

## Check

Disable alerts, simulate the upgrade path the platform documents, and confirm alerts stay off. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: If the user disabled notifications before an upgrade that introduces the runtime notification permission, that denial persists.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Check that alerts are allowed before you send one](118-check-before-you-notify.md)
