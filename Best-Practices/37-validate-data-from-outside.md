---
title: Validate data that arrives from outside
tags: [practices, security, error, state, mobile]
status: tested
updated: 2026-10-19
---

# Validate data that arrives from outside

Files, links, shares, and network responses are input. They can be the wrong shape or hostile.

## Rule

Check the type, size, and shape of data before storing or showing it. Reject what does not match, and say so on the screen when the person was waiting on it.

## Specify

- What may arrive.
- The limits.
- The screen when validation fails.

## Check

Send an oversized file and a file of the wrong type. Neither is stored as a valid record, and the screen explains the failure. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Perform input validation when handling data from external storage as you would with data from any untrusted source.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [An incoming share is validated before it is stored](89-incoming-share-is-validated.md)
- [External storage is untrusted](31-external-storage-is-untrusted.md)
