---
title: Point an error at the field
tags: [practices, error, screen, accessibility, mobile]
status: tested
updated: 2026-10-19
---

# Point an error at the field

A banner that says something failed does not say which field to fix.

## Rule

Name the field, or move focus to it, and describe what is wrong with that field. A list of errors is fine when several fields fail. Each item still names its field.

## Specify

- How each field is identified.
- What one error looks like.
- What several errors look like.

## Check

Submit a form with two invalid fields. Both are named. Fixing one leaves the other named. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 3.3.1: Error Identification](https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html). The page supports this rule: This success criterion requires that users be provided with information about the nature of the error, including the identity of the item in error.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Name an input error in text](39-name-the-input-error-in-text.md)
- [Keep what the person typed when validation fails](81-preserve-input-when-validation-fails.md)
