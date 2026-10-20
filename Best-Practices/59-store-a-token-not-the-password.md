---
title: Store a token, not the password
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Store a token, not the password

A password saved on the device is the person's credential for other places too.

## Rule

After a successful sign-in, keep a short-lived token in the platform's protected store. Do not write the password into app storage, preferences, or a backup.

## Specify

- What is stored after sign-in.
- Where it is stored.
- What sign-out removes.

## Check

Sign in and inspect app files and backups. The password is absent. The token is in the protected store. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: If you must use traditional password authentication, don't store user IDs and passwords on the device. Instead, perform initial authentication using the username and password supplied by the user, and then use a short-lived, service-specific authorization token.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Exclude secrets from backup](33-exclude-secrets-from-backup.md)
- [Keep on-device tokens short-lived](63-short-lived-tokens.md)
