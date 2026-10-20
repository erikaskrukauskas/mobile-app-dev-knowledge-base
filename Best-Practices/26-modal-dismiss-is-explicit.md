---
title: Dismissing a modal is an explicit choice
tags: [practices, navigation, screen, mobile]
status: tested
updated: 2026-10-19
---

# Dismissing a modal is an explicit choice

A sheet or dialog sits on top of a task. Dismissing it can discard a choice or commit one.

## Rule

Say what dismiss does: cancel, save a draft, or commit. The control that dismisses it, including a tap outside, matches that choice.

## Specify

- What dismiss means.
- Which gestures dismiss.
- What remains on the screen underneath.

## Check

Open the modal, enter input, and dismiss it with each allowed gesture. The underlying screen matches the specification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Navigation](https://developer.android.com/guide/navigation). The page supports this rule: Navigation includes the moves into and back out from a piece of content. A modal is one of those moves and needs a defined way back.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Back does not silently drop unsaved input](24-back-keeps-unsaved-input.md)
