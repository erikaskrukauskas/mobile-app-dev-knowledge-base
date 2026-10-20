---
title: A restore can finish before the first launch
tags: [practices, state, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# A restore can finish before the first launch

On a new device, restored files can appear before the person has opened the app. First-launch code that assumes empty storage will wipe or misread that data.

## Rule

First launch detects restored data and offers the signed-out or signed-in path the specification names. It does not delete a restored non-secret record, and it does not trust a restored secret if you excluded secrets correctly.

## Specify

- What first launch does when storage is already populated.
- What it does when storage is empty.
- That secrets are not expected to be present.

## Check

Restore a backup, then open the app for the first time. Restored non-secret records are handled. An empty install still shows the new-install path. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Back up user data with Auto Backup](https://developer.android.com/guide/topics/data/autobackup). The page supports this rule: Data is restored whenever the app is installed, and the restore operation occurs after the APK is installed but before the app is available to be launched by the user.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Test backup and restore](98-test-backup-and-restore.md)
- [Exclude secrets from backup](33-exclude-secrets-from-backup.md)
