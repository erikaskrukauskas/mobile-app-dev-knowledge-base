---
title: Focus location is exposed to assistive technology
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# Focus location is exposed to assistive technology

People navigating by switch or keyboard need to know which control has focus.

## Rule

The focused control is exposed as focused, and a focus move is available to assistive technology. A custom draw that looks focused but does not expose focus fails this.

## Specify

- How focus is shown.
- How it is exposed.
- Where focus goes when a dialog opens and when it closes.

## Check

Move focus with a keyboard or screen reader. The focused control is the one announced. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: Whether or not a control has focus can be programmatically determined, and notifications about change of focus are sent to assistive technology.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Focus order follows the task](69-focus-order.md)
