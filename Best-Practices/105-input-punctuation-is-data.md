---
title: Punctuation in input is data, not a command
tags: [practices, security, error, screen, mobile]
status: tested
updated: 2026-10-19
---

# Punctuation in input is data, not a command

Search boxes and names contain apostrophes, quotes, and characters that are special in a query language.

## Rule

Treat that input as data. The screen either finds the literal text or says it found nothing. It does not error with a store failure.

## Specify

- The characters you accept as data.
- The message when nothing matches.
- The message when the input is actually too long.

## Check

Search for a name that contains an apostrophe and a quote. The store does not error. The result is the literal match or the empty message. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Using parameterized methods is not sufficient if the selection argument is built by concatenating user data. Bind the data instead.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Query local structured stores with parameters](93-parameterized-local-queries.md)
