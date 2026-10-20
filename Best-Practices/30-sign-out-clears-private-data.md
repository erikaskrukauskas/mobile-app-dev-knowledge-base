---
title: Sign-out clears private local data
tags: [practices, security, state, offline, mobile]
status: tested
updated: 2026-10-19
---

# Sign-out clears private local data

A later person who opens the app on the same device should not see the previous person's private cache, drafts, or tokens.

## Rule

Sign-out removes private local data for that account: tokens, cached private records, and drafts. Say what, if anything, is deliberately kept on the device.

## Specify

- What is removed.
- What is kept, and why.
- What the next launch shows.

## Check

Sign in, create a private draft, sign out, and sign in as someone else. The draft and the previous token are gone. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Make sure that you don't inadvertently expose user data to other applications on the device. The same duty applies to the next person who uses the device.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [One account's local data is not another's](83-accounts-do-not-share-local-data.md)
- [Mobile application security](06-mobile-application-security.md)
