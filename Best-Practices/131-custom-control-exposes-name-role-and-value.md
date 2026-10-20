---
title: A custom control exposes its name, role, and value
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A custom control exposes its name, role, and value

A control drawn as a picture is invisible to a screen reader unless the platform is told what it is.

## Rule

For a custom control, expose the name, the role, and the value or state. Prefer a platform control that already does this. A screen reader can activate it and hear when the value changes.

## Specify

- The name.
- The role.
- The value or state.
- How a change is announced.

## Check

Focus the custom control with a screen reader. The name, role, and value are spoken. Change the value and the change is announced. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: The name and role can be programmatically determined; states, properties, and values that can be set by the user can be programmatically set; and notification of changes is available to assistive technologies.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The accessible name matches the visible label](70-label-matches-visible-text.md)
