---
title: Precise location is a separate, narrower need
tags: [practices, permissions, security, mobile]
status: tested
updated: 2026-10-19
---

# Precise location is a separate, narrower need

A nearby-store feature and a turn-by-turn feature do not need the same precision.

## Rule

Request the coarsest location that makes the screen true. Ask for precise location only for the action that fails without it, and say why.

## Specify

- The action that is correct with coarse location.
- The action that needs precise location.
- The reason shown for the precise request.

## Check

Use the coarse feature and confirm precise location was not requested. Use the precise feature and confirm the reason is shown. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: Restricting access to sensitive permissions reduces risk. Request only what the action needs, at the time of the action.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Request the smallest permission](44-smallest-permission.md)
- [Access while the app is hidden is a separate decision](49-special-access-is-separate.md)
