---
title: Cache is not the record
tags: [practices, offline, state, mobile]
status: tested
updated: 2026-10-19
---

# Cache is not the record

A cache directory is excluded from backup and may be cleared. It cannot be the only place a record exists.

## Rule

Use cache for data you can fetch or rebuild. The record of user work and of pending commands lives somewhere else.

## Specify

- What is cache.
- What is the record.
- What a cleared cache changes on screen.

## Check

Clear cache and reopen the app. Rebuildable data can reload. User work and pending commands remain. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Back up user data with Auto Backup](https://developer.android.com/guide/topics/data/autobackup). The page supports this rule: Auto Backup excludes the cache directory. The files saved there are needed only temporarily and are intentionally excluded from backup.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [User work is not cache](28-user-work-is-not-cache.md)
