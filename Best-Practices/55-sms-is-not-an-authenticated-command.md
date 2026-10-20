---
title: An SMS is not an authenticated command
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# An SMS is not an authenticated command

A text message can be spoofed, and other apps that can read messages can see it.

## Rule

Do not sign the person in, reset access, or change a sensitive setting because an SMS arrived. Use a channel that authenticates the sender.

## Specify

- Which messages the app may read, if any.
- What those messages are allowed to change.
- What a sensitive change requires instead.

## Check

Deliver an SMS that looks like a command. The sensitive action does not run. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Don't rely on unauthenticated SMS data to perform sensitive commands.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [An unverified link is not the caller's identity](20-unverified-link-is-not-identity.md)
