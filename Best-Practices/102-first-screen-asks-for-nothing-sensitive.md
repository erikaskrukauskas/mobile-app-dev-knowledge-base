---
title: The first screen does not ask for sensitive access
tags: [practices, permissions, screen, mobile]
status: tested
updated: 2026-10-19
---

# The first screen does not ask for sensitive access

The first screen is where the person decides whether to stay. A permission prompt is a poor greeting.

## Rule

The first screen completes without a permission prompt. Prompts wait for the action that needs them, as in [Ask for a permission at the action](48-ask-at-the-action.md).

## Specify

- What the first screen shows.
- The permissions it does not request.

## Check

Install and open the app. Reach the first useful screen with no permission prompt. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: Request permissions as late into the flow as possible. For example, wait until the person has started the action that needs the microphone.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Ask for a permission at the action](48-ask-at-the-action.md)
