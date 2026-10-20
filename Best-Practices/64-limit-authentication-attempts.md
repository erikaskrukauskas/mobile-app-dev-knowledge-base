---
title: Limit repeated authentication attempts on the device
tags: [practices, security, screen, mobile]
status: tested
updated: 2026-10-19
---

# Limit repeated authentication attempts on the device

A screen that accepts unlimited password or code attempts helps someone who holds the unlocked phone.

## Rule

Slow or stop repeated failures, and say so on the screen. Keep the limit in a range a person who mistyped can still pass. The server-side rule for credential guessing, if there is one, lives in the application-development knowledge base.

## Specify

- How many failures are allowed.
- What the screen shows when the limit is hit.
- When attempts are allowed again.

## Check

Fail the check until the limit. The screen stops accepting attempts and says when to retry. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Rapid, successive authentication or authorization requests can be a sign of a brute-force attack. Limit these rates to a reasonable frequency while still allowing for a functional and user-friendly app experience.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Store a token, not the password](59-store-a-token-not-the-password.md)
