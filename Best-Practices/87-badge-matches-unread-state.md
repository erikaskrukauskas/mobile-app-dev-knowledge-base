---
title: A badge matches the unread state
tags: [practices, screen, state, mobile]
status: tested
updated: 2026-10-19
---

# A badge matches the unread state

A badge that stays after the person has read the item teaches them to ignore it.

## Rule

The badge count equals the unread state the screen shows. Opening the item, or marking it read, updates the badge. Clearing the badge without changing the state is not the rule.

## Specify

- What counts as unread.
- When the badge updates.
- What zero looks like.

## Check

Read the item. The badge drops. Mark it unread again and the badge returns. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: Users expect UI state to match what they just did. A badge is UI state for unread items.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A notification opens the screen that holds the state](85-notification-opens-the-state.md)
