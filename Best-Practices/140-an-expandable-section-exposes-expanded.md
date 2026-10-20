---
title: An expandable section exposes whether it is open
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# An expandable section exposes whether it is open

A row that opens more content is a state, not only a tap target.

## Rule

Expose expanded or collapsed, and announce the change. The content that appears is in the focus order.

## Specify

- The sections.
- The state.
- Where focus goes when one opens.

## Check

Expand and collapse a section with a screen reader. The state is spoken and the new content can be reached. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: A collapsible section's expanded or collapsed state is an example of a state assistive technology needs.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Focus order follows the task](69-focus-order.md)
