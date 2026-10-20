---
title: A pressed or selected control exposes that state
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A pressed or selected control exposes that state

A toggle that only changes color is the color-only problem again, and a screen reader never hears it.

## Rule

Expose pressed, selected, or checked in addition to any color change. The text or the state is enough to tell them apart with the screen off.

## Specify

- The controls.
- The exposed state.

## Check

Activate the control with a screen reader. The new state is spoken, not only a color change. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: Selected and checked are states assistive technologies need. Color can sit beside that state. It does not replace it.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A status icon also has text](72-status-icons-have-text.md)
- [A control's state is available, not only its label](132-a-control-state-is-part-of-the-name.md)
