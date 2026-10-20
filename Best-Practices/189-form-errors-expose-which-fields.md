---
title: A form error exposes which fields are invalid
tags: [practices, accessibility, error, mobile]
status: tested
updated: 2026-10-19
---

# A form error exposes which fields are invalid

A summary that says two errors is not enough if the fields themselves do not carry the invalid state.

## Rule

Each invalid field exposes invalid, and the summary or the focus move lets them reach those fields. Fixing a field clears its own state without clearing the others.

## Specify

- The summary.
- The per-field state.
- The focus move.

## Check

Submit two invalid fields with a screen reader. Both are reachable and marked invalid. Fix one. The other stays invalid. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: States of components, and changes to those states, are available to assistive technologies. Error identification still has to name the field in text.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Point an error at the field](40-name-the-field-that-failed.md)
- [An invalid field exposes an invalid state](158-an-invalid-field-exposes-invalid.md)
