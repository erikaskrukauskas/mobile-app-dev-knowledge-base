---
title: Backup is not the only copy
tags: [practices, state, offline, mobile]
status: tested
updated: 2026-10-19
---

# Backup is not the only copy

Backup runs only when the device is idle, on a network, and under a size limit. It can fail or never run.

## Rule

Do not treat platform backup as the save that protects user work. Write user work to its real store. Backup is a convenience copy of non-secret data.

## Specify

- The store that is the real record.
- What may also be in a backup.
- What the person can still do if backup never ran.

## Check

Save user work, then simulate a device with backup disabled. The work is still available from its real store. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Back up user data with Auto Backup](https://developer.android.com/guide/topics/data/autobackup). The page supports this rule: If the amount of data is over 25 MB, the system does not back up data to the cloud. A device might never back up if it never connects to a network.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [User work is not cache](28-user-work-is-not-cache.md)
- [Exclude secrets from backup](33-exclude-secrets-from-backup.md)
