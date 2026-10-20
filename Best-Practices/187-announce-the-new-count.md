---
title: A changed count is announced when it is the point
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A changed count is announced when it is the point

A badge that changes from one to two while they are on the screen can be the whole point of the screen, or it can be noise.

## Rule

If the count is the task, announce the new count. If it is incidental, update it quietly. Do not announce every tick of a spinner.

## Specify

- The counts that are announced.
- The ones that are quiet.

## Check

Change an announced count with a screen reader on. It is spoken once. A spinner tick is not. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: Notification of changes is for state the person needs. Not every visual tick is a change assistive technology must speak, but a meaningful value change is available.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A live update is announced when it changes the task](142-a-live-update-is-announced-when-it-matters.md)
- [A badge matches the unread state](87-badge-matches-unread-state.md)
