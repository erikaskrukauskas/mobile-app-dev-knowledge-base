---
title: Tokens are not copied into before-unlock storage
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Tokens are not copied into before-unlock storage

Moving a token so an alarm can see it also leaves the token available before the person unlocks the phone.

## Rule

Do not migrate tokens, passwords, or private records into the storage that exists before unlock. Migrate only the non-secret data a before-unlock task truly needs.

## Specify

- What may be migrated.
- What must not.
- How the after-unlock path reads the token.

## Check

Inspect before-unlock storage after sign-in and a reboot. The token is absent there. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: Don't migrate private user information, such as passwords or authorization tokens, from credential encrypted storage to device encrypted storage.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Store a token, not the password](59-store-a-token-not-the-password.md)
- [Private data waits until the device is unlocked](116-private-data-waits-for-unlock.md)
