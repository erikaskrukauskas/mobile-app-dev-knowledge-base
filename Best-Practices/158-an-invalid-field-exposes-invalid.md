---
title: An invalid field exposes an invalid state
tags: [practices, accessibility, error, mobile]
status: tested
updated: 2026-10-19
---

# An invalid field exposes an invalid state

Error text next to a field can be missed if the field itself does not carry the invalid state.

## Rule

Mark the field invalid when its error is showing, and clear that state when the value becomes valid. Keep the text from the error rule as well.

## Specify

- When the field is invalid.
- The text.
- When the state clears.

## Check

Submit an invalid field with a screen reader. The field is announced as invalid and the text is available. Correct it and the invalid state is gone. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: States and properties of a component are available to assistive technologies, and changes to those items are notified.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Point an error at the field](40-name-the-field-that-failed.md)
- [An error is announced](71-error-is-announced.md)
