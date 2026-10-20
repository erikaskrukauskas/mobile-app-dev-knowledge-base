---
title: Multi-window keeps the screen's state
tags: [practices, lifecycle, screen, state, mobile]
status: tested
updated: 2026-10-19
---

# Multi-window keeps the screen's state

Split screen is a configuration change the person can do without meaning to restart the task.

## Rule

Entering and leaving multi-window keeps the same input and the same place in the task.

## Specify

- The state that must survive.
- The devices or emulators that support split screen.

## Check

Fill a field, enter split screen, and return to full screen. The field value is unchanged. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: A user expects a screen's UI state to remain the same throughout a configuration change, such as rotation or switching into multi-window mode.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Keep input across a configuration change](11-keep-state-across-configuration-change.md)
