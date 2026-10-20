---
title: A live update is announced when it changes the task
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A live update is announced when it changes the task

A new message or a finished upload can appear away from the focused control.

## Rule

Announce an update that changes what the person needs to do or know. Do not announce every quiet refresh. The announcement is the same text the screen shows.

## Specify

- Which updates are announced.
- Which refreshes stay quiet.
- The text of the announcement.

## Check

Trigger a meaningful update while focus is elsewhere and a screen reader is on. It is announced once. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: Notification of changes to names, roles, states, and values is available to assistive technologies.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [An error is announced](71-error-is-announced.md)
