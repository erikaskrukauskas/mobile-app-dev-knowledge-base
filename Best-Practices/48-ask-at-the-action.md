---
title: Ask for a permission at the action
tags: [practices, permissions, screen, mobile]
status: tested
updated: 2026-10-19
---

# Ask for a permission at the action

A prompt at first launch asks for access the person has not tried to use.

## Rule

Request the permission when they attempt the action that needs it. Do not bundle later permissions into the first screen.

## Specify

- The action that triggers the prompt.
- The first screen, which does not prompt for that action.
- What the first screen can do without the permission.

## Check

Cold-start the app and reach the first screen without a prompt. Attempt the action and the prompt appears then. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: Request permissions as late into the flow of your app's use cases as possible.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Request the smallest permission](44-smallest-permission.md)
- [The first screen does not wait on a permission](104-first-screen-does-not-wait-on-a-permission.md)
