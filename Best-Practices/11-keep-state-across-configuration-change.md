---
title: Keep input across a configuration change
tags: [practices, lifecycle, screen, state, mobile]
status: tested
updated: 2026-10-19
---

# Keep input across a configuration change

Rotation, resizing, and multi-window are not a new visit. The person expects the same input and the same place in the task.

## Rule

A configuration change keeps what they typed, what they selected, and where they were. Rebuilding the screen from empty on rotation is a failed check.

## Specify

- Which configuration changes the screen must survive.
- Which fields and selections are kept.
- That the first frame after the change does not wait on a full network reload when the state is already local.

## Check

Rotate the device, or move the app into a split view, in the middle of an edit. The input is still there. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: A user expects a screen's UI state to remain the same throughout a configuration change, such as rotation or switching into multi-window mode.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Save state before process death](09-save-before-process-death.md)
- [The keyboard does not cover the focused field](77-keyboard-does-not-cover-the-field.md)
