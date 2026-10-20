---
title: Read private storage only after unlock
tags: [practices, security, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Read private storage only after unlock

A restart can deliver a boot event before the person has unlocked the phone.

## Rule

Check that the user is unlocked before reading private storage. If they are not, do the small before-unlock task only, or wait.

## Specify

- The check.
- The branch before unlock.
- The branch after unlock.

## Check

Reboot and trigger the app before unlock. Private storage is not read. Unlock and the private path runs. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: If the user has unlocked the device, you can find out by calling the user-unlocked check. Credential encrypted storage is available after unlock.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Private data waits until the device is unlocked](116-private-data-waits-for-unlock.md)
