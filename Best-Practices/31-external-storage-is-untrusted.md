---
title: External storage is untrusted
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# External storage is untrusted

Storage the person can remove, or that other apps can read, is not a private store.

## Rule

Keep sensitive and private data out of external storage. Treat anything read from it as untrusted input.

## Specify

- What may be written there.
- What must not.
- How data read from it is checked.

## Check

Confirm a private record is not in the external store. Read a modified file from that store and confirm the app rejects or isolates it. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Because external storage can be removed by the user and also modified by any application, only store non-sensitive information using external storage.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Private files stay in app storage](32-private-files-stay-in-app-storage.md)
- [Validate data that arrives from outside](37-validate-data-from-outside.md)
