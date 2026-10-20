---
title: A slider or progress control exposes its value
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A slider or progress control exposes its value

A slider the person can move, or a progress indicator they are waiting on, has a value. A silent graphic does not.

## Rule

Expose the current value and announce changes. If progress is indeterminate, expose that it is working, not a fake percent.

## Specify

- The control.
- The value or the working state.
- The announcement when it changes.

## Check

Move the slider, or watch progress, with a screen reader. The value or the working state is announced. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: Values that can be set by the user can be programmatically set, and changes are available to assistive technologies.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A loading screen says it is waiting](80-loading-state-says-waiting.md)
- [A control's state is available, not only its label](132-a-control-state-is-part-of-the-name.md)
