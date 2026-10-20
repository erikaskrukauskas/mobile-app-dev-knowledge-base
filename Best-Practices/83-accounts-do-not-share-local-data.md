---
title: One account's local data is not another's
tags: [practices, security, state, offline, mobile]
status: tested
updated: 2026-10-19
---

# One account's local data is not another's

Two accounts on one phone can share a process. Their drafts and tokens must not.

## Rule

Key private local data by account, and hide the other account's data when you switch. A switch clears the previous account's tokens from memory.

## Specify

- What is stored per account.
- What a switch removes from memory.
- What the screen shows during the switch.

## Check

Create data as account A, switch to account B, and confirm A's data and token are not visible or sent. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: The security guidance is to avoid exposing user data through overly permissive storage. A second account on the same install is another reader.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Sign-out clears private local data](30-sign-out-clears-private-data.md)
