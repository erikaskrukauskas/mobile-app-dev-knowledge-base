---
title: Work before unlock is a small, explicit component
tags: [practices, lifecycle, security, mobile]
status: tested
updated: 2026-10-19
---

# Work before unlock is a small, explicit component

The whole app should not run on a locked device. A clock alarm or an accessibility service sometimes must.

## Rule

If something must run before unlock, register that component on purpose and limit it to the task. Everything else waits. The before-unlock task does not read private records.

## Specify

- The component that may run.
- The data it may read.
- The rest of the app, which does not run yet.

## Check

Reboot and leave the device locked. Only the named component runs, and it does not show private content. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: By default, apps don't run during Direct Boot. Components that must run are marked encryption aware. Use device encrypted storage only for information that must be accessible during Direct Boot.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Private data waits until the device is unlocked](116-private-data-waits-for-unlock.md)
