---
title: Keep on-device tokens short-lived
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Keep on-device tokens short-lived

A token on the device will be copied if the device is. A long-lived token makes that copy useful.

## Rule

Use a token that expires, and refresh it. Do not store a token that grants broad access for longer than the screen's specification allows.

## Specify

- The token lifetime.
- What refresh does.
- What the screen does when refresh fails.

## Check

Expire the token and open a private screen. The app refreshes or asks the person to sign in. The old token does not keep working past its lifetime. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Limit access tokens. Use short-lived tokens for operations and API calls. Avoid unnecessary credential requests. Instead, use an authorization token and refresh it.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Store a token, not the password](59-store-a-token-not-the-password.md)
