---
title: Test a configuration change in the middle of input
tags: [practices, testing, lifecycle, screen, mobile]
status: tested
updated: 2026-10-19
---

# Test a configuration change in the middle of input

Rotation is the check people skip because the simulator is already in portrait.

## Rule

Rotate, or enter multi-window, while a field is focused and filled. The input remains, as [Keep input across a configuration change](11-keep-state-across-configuration-change.md) requires.

## Specify

- The device.
- The field.
- The expected text after the change.

## Check

Run the change in the middle of typing. The text is still in the field. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: By default the system destroys the host activity on a configuration change. The test shows whether your save made that destruction invisible.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Keep input across a configuration change](11-keep-state-across-configuration-change.md)
