---
title: An error is announced
tags: [practices, accessibility, error, screen, mobile]
status: tested
updated: 2026-10-19
---

# An error is announced

A text error that appears away from the current focus can be invisible to a screen reader.

## Rule

When an error appears, move focus to it or announce it. The announcement includes the text from [Name an input error in text](39-name-the-input-error-in-text.md).

## Specify

- What is announced.
- Where focus goes.
- What happens when there are several errors.

## Check

Trigger an error with the screen reader on. The error text is announced without a manual hunt. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 3.3.1: Error Identification](https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html). The page supports this rule: The identification and description of an error can be combined with programmatic information that assistive technologies can use to identify an error.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Name an input error in text](39-name-the-input-error-in-text.md)
