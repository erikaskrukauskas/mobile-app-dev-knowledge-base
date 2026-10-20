---
title: System bars do not cover the controls
tags: [practices, screen, accessibility, mobile]
status: tested
updated: 2026-10-19
---

# System bars do not cover the controls

A notch, a status bar, a navigation bar, or a home indicator can cover a control placed at the edge.

## Rule

Keep essential controls and text inside the area the platform says is safe. Confirm the current inset guidance before you hard-code an offset.

## Specify

- Which controls are essential.
- The insets the layout respects.
- The devices the check uses, including one with a home indicator or a tall status area.

## Check

On a device with a system bar that overlaps content, every essential control can be read and tapped. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Build accessible apps](https://developer.android.com/guide/topics/ui/accessibility). The page supports this rule: Touch targets and reachable flows are part of the Android accessibility guide. A control under a system bar fails that flow.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Make touch targets large enough or far enough apart](65-target-size-or-spacing.md)
