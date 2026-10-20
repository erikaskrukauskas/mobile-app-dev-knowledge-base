---
title: A complex gesture has a simple alternative
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A complex gesture has a simple alternative

A swipe, a long-press, or a multi-finger gesture is invisible and may be impossible.

## Rule

Every action that uses a complex gesture also has a visible control that does the same thing. The control's name says what it does.

## Specify

- The gestures.
- The visible alternative for each.
- The accessible name of that control.

## Check

Complete the action with the visible control and without the gesture, using a screen reader. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Build accessible apps](https://developer.android.com/guide/topics/ui/accessibility). The page supports this rule: The Android accessibility guide requires user flows to be accessible, which includes a way to operate the flow without a gesture the assistive technology cannot perform.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The accessible name matches the visible label](70-label-matches-visible-text.md)
- [Back returns to the previous place](17-back-returns-to-previous.md)
