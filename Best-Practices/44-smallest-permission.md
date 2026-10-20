---
title: Request the smallest permission
tags: [practices, permissions, security, mobile]
status: tested
updated: 2026-10-19
---

# Request the smallest permission

A permission is access to restricted data or a restricted action. Extra access is extra harm if the app is misused.

## Rule

Request only the permission the action needs. If the action can be done with a picker or another path that needs no permission, use that path.

## Specify

- The action.
- The permission, or the path that needs none.
- What is not requested.

## Check

Complete the action and inspect the permissions the app holds. The unused ones are absent. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: If you decide that your app must access restricted data or perform restricted actions to fulfill a use case, declare the appropriate permissions. The same guide says to request a minimal number of permissions.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Picking one item does not need the whole library](90-one-item-does-not-need-the-library.md)
- [Mobile application security](06-mobile-application-security.md)
