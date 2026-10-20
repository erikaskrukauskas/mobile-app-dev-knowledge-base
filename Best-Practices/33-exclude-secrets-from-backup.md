---
title: Exclude secrets from backup
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Exclude secrets from backup

A platform backup can copy app files to the person's account. A token in those files leaves the device.

## Rule

Exclude credentials, tokens, and other secrets from backup. Confirm the platform's exclude mechanism before relying on a directory name.

## Specify

- Which files are secrets.
- How they are excluded.
- What a restore on a new device must ask the person to do again.

## Check

Back up and restore onto a second install. Secrets are not in the restored files, and the person can sign in again. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Back up user data with Auto Backup](https://developer.android.com/guide/topics/data/autobackup). The page supports this rule: Auto Backup includes shared preferences, internal files, and databases by default, and excludes cache and the no-backup directory. Secrets in the included set are backed up unless you exclude them.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Backup is not the only copy](34-backup-is-not-the-only-copy.md)
- [Store a token, not the password](59-store-a-token-not-the-password.md)
