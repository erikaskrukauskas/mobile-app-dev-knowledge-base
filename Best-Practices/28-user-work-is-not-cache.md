---
title: User work is not cache
tags: [practices, offline, state, security, mobile]
status: tested
updated: 2026-10-19
---

# User work is not cache

Cache is disposable. A draft, a photo they took, or a message they have not sent is not disposable.

## Rule

Put the only copy of user work in a store that the system does not treat as cache. Cache may hold copies that can be fetched again.

## Specify

- Which data is user work.
- Which store holds it.
- What a cache clear is allowed to delete.

## Check

Clear the cache, or let the system reclaim it, and reopen the draft. The draft is still there. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Back up user data with Auto Backup](https://developer.android.com/guide/topics/data/autobackup). The page supports this rule: Auto Backup excludes files in the cache directory and the no-backup directory. Those locations are for data needed only temporarily.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Keep process-death state small](16-small-saved-state.md)
- [Exclude secrets from backup](33-exclude-secrets-from-backup.md)
