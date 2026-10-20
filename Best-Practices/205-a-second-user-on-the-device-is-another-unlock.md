---
title: Another user on the device is another unlock
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Another user on the device is another unlock

Some devices have more than one user. Their credential stores are not yours to read while they are locked.

## Rule

Read private data only for the unlocked user you are serving. Do not keep another user's token in a store that is available before that user unlocks.

## Specify

- Which user's data is readable now.
- What is not.

## Check

Switch users or lock the other user and confirm their private records are not shown. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: File-based encryption with Direct Boot is per user. Credential storage for a user is available after that user unlocks.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [One account's local data is not another's](83-accounts-do-not-share-local-data.md)
