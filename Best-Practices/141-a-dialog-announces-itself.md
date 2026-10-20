---
title: A dialog announces itself and returns focus
tags: [practices, accessibility, navigation, screen, mobile]
status: tested
updated: 2026-10-19
---

# A dialog announces itself and returns focus

A sheet that appears without moving focus is invisible to a screen reader. When it closes, focus should not fall on a random control.

## Rule

When a dialog opens, focus moves inside it and its role is a dialog. When it closes, focus returns to the control that opened it.

## Specify

- The opener.
- The first focused control inside.
- The control focused after close.

## Check

Open and close the dialog with a screen reader. Focus moves in, the dialog is announced, and focus returns. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: Focus location can be determined, and focus changes are sent to assistive technology. A custom component still has to expose its role.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Dismissing a modal is an explicit choice](26-modal-dismiss-is-explicit.md)
- [Focus location is exposed to assistive technology](133-focus-itself-is-exposed.md)
