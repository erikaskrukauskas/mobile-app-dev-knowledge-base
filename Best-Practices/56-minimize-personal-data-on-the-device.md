---
title: Keep as little personal data on the device as the screen needs
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Keep as little personal data on the device as the screen needs

A copy on the device is a copy that backup, logs, and the next user of the phone can expose.

## Rule

Store and show the personal data the screen needs, and no more. Prefer a non-reversible form when the screen does not need the original value.

## Specify

- What is stored.
- Why each field is needed on the device.
- When it is removed.

## Check

Inspect the local store after the main task. Fields the screen does not need are absent. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: If you have access to user data, avoid storing or transmitting it if you can. Consider whether your application logic can be implemented using a hash or non-reversible form of the data.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Sign-out clears private local data](30-sign-out-clears-private-data.md)
- [Exclude secrets from backup](33-exclude-secrets-from-backup.md)
