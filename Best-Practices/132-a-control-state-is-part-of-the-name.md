---
title: A control's state is available, not only its label
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A control's state is available, not only its label

A switch that only says Notifications can be on or off. The label alone hides which.

## Rule

Expose state such as selected, checked, or expanded. When it changes, assistive technology can hear the new state.

## Specify

- The states each control has.
- The announcement when one changes.

## Check

Toggle the control with a screen reader. The spoken result includes the new state. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: Examples of states are whether a checkbox or radio button is selected, or whether a collapsible section is expanded or collapsed. Changes to these items are available to assistive technologies.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A custom control exposes its name, role, and value](131-custom-control-exposes-name-role-and-value.md)
