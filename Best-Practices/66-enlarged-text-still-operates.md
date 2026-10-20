---
title: Enlarged text still operates the screen
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# Enlarged text still operates the screen

A person who enlarges text still has to reach every control and read every name.

## Rule

At the largest text size you support, controls are visible, labels are not clipped into nonsense, and the main action can be reached. Scrolling the screen is acceptable. A control that sits off-screen with no way to reach it is not.

## Specify

- The text sizes the screen supports.
- What may scroll.
- What must remain reachable.

## Check

Set the device text size to the largest supported value and complete the main path. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Build accessible apps](https://developer.android.com/guide/topics/ui/accessibility). The page supports this rule: The Android accessibility guide points to text and content labeling, and to testing flows, as part of building apps people can use. Enlarged text is one of those flows.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Make touch targets large enough or far enough apart](65-target-size-or-spacing.md)
- [System bars do not cover the controls](78-safe-area-keeps-controls-reachable.md)
