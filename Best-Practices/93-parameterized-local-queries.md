---
title: Query local structured stores with parameters
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Query local structured stores with parameters

A local database is still a database. Building a query by gluing text from a link or a search box is injection.

## Rule

Pass input as parameters. Do not concatenate it into the query text. Limit the operation to read or write when that is all the screen needs.

## Specify

- The queries the screen runs.
- How input is bound.
- What a hostile string does.

## Check

Enter a search that contains query punctuation. The search treats it as text. It does not change the store. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: When accessing a content provider, use parameterized query methods to avoid potential SQL injection from untrusted sources.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Validate data that arrives from outside](37-validate-data-from-outside.md)
