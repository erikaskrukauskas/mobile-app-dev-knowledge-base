---
title: Do not only redisplay the screen after a failure
tags: [practices, error, screen, mobile]
status: tested
updated: 2026-10-19
---

# Do not only redisplay the screen after a failure

Putting the same screen back with no change hides the failure.

## Rule

A failed submit, save, or send leaves a visible text change. The input they entered stays so they can correct it.

## Specify

- What changes on screen after failure.
- What input is kept.
- What a success state looks like, so it is not the same as failure.

## Check

Fail a submit. The input remains and a text error appears. Succeed on the next try and the success state is different. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 3.3.1: Error Identification](https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html). The page supports this rule: In the case of an unsuccessful form submission, it is not sufficient to only re-display the form without providing any hint that the submission failed.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Name an input error in text](39-name-the-input-error-in-text.md)
- [Keep what the person typed when validation fails](81-preserve-input-when-validation-fails.md)
