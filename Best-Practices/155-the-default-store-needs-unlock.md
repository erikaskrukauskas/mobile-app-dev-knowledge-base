---
title: The default store is the one that needs unlock
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# The default store is the one that needs unlock

The convenient default is the private store that appears after unlock. The before-unlock store is the special case.

## Rule

Put ordinary app data in the default store. Use the before-unlock store only for the explicit exception.

## Specify

- The default location.
- The exception list.

## Check

Save an ordinary record and confirm it is not in the before-unlock store. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: Credential encrypted storage is the default storage location and is only available after the user has unlocked the device. Don't use device encrypted storage as a general-purpose encrypted store.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Private files stay in app storage](32-private-files-stay-in-app-storage.md)
