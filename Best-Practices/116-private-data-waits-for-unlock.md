---
title: Private data waits until the device is unlocked
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Private data waits until the device is unlocked

After a restart, the device can be on while the lock screen is still up. Storage that needs the person's credential is not available yet.

## Rule

Keep private records, tokens, and drafts in storage that becomes available only after unlock. Do not copy them into the storage that exists before unlock just so a background component can read them.

## Specify

- What is private.
- Where it is stored.
- What, if anything, is allowed to exist before unlock.

## Check

Reboot, stay on the lock screen, and confirm private records are not readable. Unlock and confirm they are. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: Credential encrypted storage is the default and is available only after the user has unlocked the device. Don't migrate private user information, such as passwords or authorization tokens, into device encrypted storage.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Store a token, not the password](59-store-a-token-not-the-password.md)
