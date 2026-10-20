---
title: Test a reboot that stays locked
tags: [practices, testing, security, mobile]
status: tested
updated: 2026-10-19
---

# Test a reboot that stays locked

A test that unlocks immediately never sees the before-unlock path.

## Rule

Reboot, leave the device locked, and confirm private data is unavailable and only the explicit before-unlock component runs. Then unlock and confirm private data returns.

## Specify

- The device.
- The locked checks.
- The unlocked checks.

## Check

Run both phases. They match the before-unlock and after-unlock rules. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: Test your encryption-aware app with Direct Boot enabled. Credential encrypted storage is unavailable until the user unlocks the device.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Work before unlock is a small, explicit component](117-before-unlock-work-is-explicit.md)
- [Verify on a mobile client, then record](04-verify-and-record.md)
