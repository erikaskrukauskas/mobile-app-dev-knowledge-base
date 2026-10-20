---
title: Name an input error in text
tags: [practices, error, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# Name an input error in text

Color, a shake, or a redisplayed form does not tell someone what failed.

## Rule

When the screen rejects input, identify the failure in text. The text can sit with a color or an icon. The text is what the person and a screen reader can use.

## Specify

- The errors the screen can detect.
- The text for each.
- Where the text appears.

## Check

Submit an invalid field with a screen reader on. The error is spoken or readable as text, and the field is identifiable. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 3.3.1: Error Identification](https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html). The page supports this rule: It is not sufficient to only re-display the form without providing any hint that the submission failed. The error must be indicated in text.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Point an error at the field](40-name-the-field-that-failed.md)
- [Mobile accessibility](07-mobile-accessibility.md)
