---
title: Recheck a permission before each use
tags: [practices, permissions, security, mobile]
status: tested
updated: 2026-10-19
---

# Recheck a permission before each use

A grant can be removed in system settings while the app is installed.

## Rule

Check the permission at the moment of use. Do not remember a grant from install time or from the previous session and skip the check.

## Specify

- Where the check runs.
- What happens when the grant is gone.
- What happens when it is present.

## Check

Grant the permission, revoke it in system settings, and return to the action. The app notices the revocation and follows the denial path. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: Don't assume that these permissions have been previously granted — check them and, if needed, request them before each access.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A denied permission is explained in text](42-permission-failure-is-text.md)
