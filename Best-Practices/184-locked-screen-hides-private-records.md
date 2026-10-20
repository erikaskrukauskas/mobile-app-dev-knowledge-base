---
title: The locked device does not show private records
tags: [practices, security, screen, mobile]
status: tested
updated: 2026-10-19
---

# The locked device does not show private records

A notification or a widget that renders a private record on the lock screen publishes it before unlock.

## Rule

Before unlock, show at most a generic status. The private record appears after unlock, inside the app.

## Specify

- What may show before unlock.
- What waits.

## Check

Lock the device with a private record pending. The lock screen does not show the record. Unlock and the app does. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: Private information stays in credential encrypted storage, which is unavailable until unlock. Device-encrypted storage is not a place to stage that information for display.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The visible ongoing status carries no secrets](172-visible-status-carries-no-secrets.md)
- [Private data waits until the device is unlocked](116-private-data-waits-for-unlock.md)
