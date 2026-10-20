---
title: Backup is not a save button
tags: [practices, state, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Backup is not a save button

The platform backup may skip an app that is in the foreground, and it runs on a schedule, not when the person taps Save.

## Rule

Save user work at the moment they commit it, to the store you control. Do not tell them a save succeeded because a later backup might copy the file.

## Specify

- When the app writes the record.
- What the screen calls a save.
- That backup is not that signal.

## Check

Save a record, then inspect the store before any backup runs. The record is already there. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Back up user data with Auto Backup](https://developer.android.com/guide/topics/data/autobackup). The page supports this rule: By default, the backup system ignores apps that are running in the foreground. Backups occur when the device is idle, on a network, and enough time has passed.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Backup is not the only copy](34-backup-is-not-the-only-copy.md)
