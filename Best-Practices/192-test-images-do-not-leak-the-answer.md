---
title: A test image is identified without spoiling it
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A test image is identified without spoiling it

Some images are the question. A description that gives the answer makes the question pointless, and no description makes it impossible.

## Rule

Identify the image enough to know there is a question, and provide another mode when the image itself cannot be used. Do not put the answer in the alternative.

## Specify

- The identification.
- The other mode.
- What the alternative must not include.

## Check

Open the question with a screen reader. The person can tell there is a question and can use the other mode. The answer is not in the name. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 1.1.1: Non-text Content](https://www.w3.org/WAI/WCAG22/Understanding/non-text-content.html). The page supports this rule: If non-text content is a test that would be invalid if presented in text, the text alternative at least provides descriptive identification.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A human-check has more than one sense](137-a-captcha-has-another-sense.md)
