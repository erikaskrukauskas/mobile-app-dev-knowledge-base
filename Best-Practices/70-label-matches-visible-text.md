---
title: The accessible name matches the visible label
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# The accessible name matches the visible label

A button that shows Save and is spoken as Button can be reached, but not understood.

## Rule

The name a screen reader speaks includes the visible label. If there is no visible label, the accessible name is the same words the design would have shown.

## Specify

- The visible label of each control.
- The accessible name.
- Icons that need a name because they have no text.

## Check

Turn on the screen reader and move through the controls. Each spoken name matches the visible label or the specified icon name. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Build accessible apps](https://developer.android.com/guide/topics/ui/accessibility). The page supports this rule: The Android accessibility guide calls out content labeling and succinctly describing each UI element.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Focus order follows the task](69-focus-order.md)
- [Mobile accessibility](07-mobile-accessibility.md)
