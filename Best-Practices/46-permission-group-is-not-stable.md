---
title: Do not depend on permission groups staying put
tags: [practices, permissions, mobile]
status: tested
updated: 2026-10-19
---

# Do not depend on permission groups staying put

Platforms group related permissions in the prompt. The grouping can change.

## Rule

Request and check the specific permission the action needs. Do not assume that a grant of one permission granted another because they shared a group.

## Specify

- The exact permission for the action.
- What is not implied by a neighboring grant.

## Check

Use the action after granting only the neighboring permission, if the platform allows that split. The action does not run on the neighbor's grant. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: Permissions can change groups without notice, so don't assume that a particular permission is grouped with any other permission.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Request the smallest permission](44-smallest-permission.md)
