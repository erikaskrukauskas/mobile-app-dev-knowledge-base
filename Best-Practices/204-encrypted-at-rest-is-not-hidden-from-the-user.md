---
title: Encryption at rest still unlocks for the person
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Encryption at rest still unlocks for the person

Storage encrypted until unlock is not a second password you invented. It unlocks when they unlock the device.

## Rule

Do not add a fake sense of safety by copying secrets into the before-unlock store because it is also encrypted. That store uses a device key, not their credential. Private secrets stay in the store that needs their unlock.

## Specify

- Which store holds secrets.
- Which store may hold a non-secret alarm time.

## Check

Compare the two stores after sign-in. Secrets are only in the post-unlock store. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: Device encrypted storage uses a key available after verified boot. Credential encrypted storage uses a key associated with the user's credentials. Don't treat device encrypted storage as the place for private user information.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Tokens are not copied into before-unlock storage](154-tokens-are-not-copied-before-unlock.md)
