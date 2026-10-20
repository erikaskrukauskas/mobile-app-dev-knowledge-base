---
title: Picking one item does not need the whole library
tags: [practices, permissions, security, mobile]
status: tested
updated: 2026-10-19
---

# Picking one item does not need the whole library

Ongoing access to every photo, contact, or file is a larger decision than choosing one item.

## Rule

When the person is picking one item, use a picker that returns that item. Do not request persistent access to the whole library for that action.

## Specify

- The action.
- The picker.
- The permission you are not requesting.

## Check

Pick one item and confirm the app did not gain ongoing access to the library. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: If possible, design your application in a way that doesn't require any permissions. Request only the permissions required to accomplish the task.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Request the smallest permission](44-smallest-permission.md)
