---
title: The first screen does not wait on a permission
tags: [practices, permissions, screen, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# The first screen does not wait on a permission

Blocking the first frame on a permission dialog hides the product behind a decision the person cannot judge yet.

## Rule

Draw the first useful screen without waiting for a grant. If a later region of that screen needs permission, that region explains the block. The rest of the screen still works.

## Specify

- What renders with no grant.
- Which region waits.
- The explanation in that region.

## Check

Open the app with every optional permission denied. The first screen is usable, and the blocked region explains itself. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: If a permission isn't required for your app to function, don't request it. Design so the app works without permissions where that is possible.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The first screen does not ask for sensitive access](102-first-screen-asks-for-nothing-sensitive.md)
