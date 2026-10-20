---
title: Test backup and restore
tags: [practices, testing, state, security, mobile]
status: tested
updated: 2026-10-19
---

# Test backup and restore

Backup rules that were never restored are a guess.

## Rule

Run a backup and a restore onto a clean install. Secrets are absent. Non-secret records you chose to include are present. Confirm the current platform's backup test tool before you name the command.

## Specify

- The tool.
- What must be present.
- What must be absent.

## Check

Restore onto a clean install and compare the store to the specification in [Exclude secrets from backup](33-exclude-secrets-from-backup.md). Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Back up user data with Auto Backup](https://developer.android.com/guide/topics/data/autobackup). The page supports this rule: To simplify testing, Android includes tools that let you manually initiate a backup of your app.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Exclude secrets from backup](33-exclude-secrets-from-backup.md)
