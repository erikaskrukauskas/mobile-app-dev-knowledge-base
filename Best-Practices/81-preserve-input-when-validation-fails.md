---
title: Keep what the person typed when validation fails
tags: [practices, screen, error, state, mobile]
status: tested
updated: 2026-10-19
---

# Keep what the person typed when validation fails

Clearing a form after a validation error makes them type it again, and they may not remember it.

## Rule

Keep the values they entered, including the invalid ones, and point at the fields to fix. A password field may be the exception you name, because keeping it has a different risk.

## Specify

- Which fields are kept.
- Which fields are cleared, and why.
- Where the error text sits relative to the kept value.

## Check

Submit an invalid form. The entered values are still in the fields. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 3.3.1: Error Identification](https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html). The page supports this rule: The error must identify the item and describe what is wrong. That only helps if the item still holds what they entered.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Point an error at the field](40-name-the-field-that-failed.md)
- [Do not only redisplay the screen after a failure](43-do-not-only-redisplay-the-screen.md)
