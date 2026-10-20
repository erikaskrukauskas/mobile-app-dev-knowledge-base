---
title: A group of fields has a name
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A group of fields has a name

Three radio options without a group name are three unrelated buttons.

## Rule

Name the group with the question the options answer. Each option still has its own name and selected state.

## Specify

- The group name.
- The option names.
- The selected state.

## Check

Move through the group with a screen reader. The question and the selected option are both announced. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: Assistive technology needs the name, role, and state of each component, including components that are a set of options.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A control's state is available, not only its label](132-a-control-state-is-part-of-the-name.md)
