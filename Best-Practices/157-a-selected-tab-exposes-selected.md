---
title: The selected section exposes that it is selected
tags: [practices, accessibility, navigation, mobile]
status: tested
updated: 2026-10-19
---

# The selected section exposes that it is selected

A row of sections that all look like buttons hides which one is current.

## Rule

Expose the selected section as selected. Changing sections announces the new selection.

## Specify

- The sections.
- The selected state.
- The announcement.

## Check

Switch sections with a screen reader. The newly selected section is announced as selected. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: Selected state is one of the states assistive technologies need, and changes to that state are notified.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Each top-level section keeps its place](22-each-section-keeps-its-place.md)
