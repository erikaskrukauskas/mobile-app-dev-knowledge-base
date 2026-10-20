---
title: A status icon also has text
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A status icon also has text

A color or an icon that means failed, waiting, or done is invisible to someone who cannot see that color.

## Rule

Every status that uses color or an icon also has text with the same meaning. The icon can stay.

## Specify

- The statuses.
- The text for each.
- Where the text appears.

## Check

Turn on a screen reader, or cover the icon, and identify each status from the text alone. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 3.3.1: Error Identification](https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html). The page supports this rule: It is perfectly acceptable to indicate the error in other ways such as through the use of an image, color, or other visual indicator, in addition to the text description.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Name an input error in text](39-name-the-input-error-in-text.md)
- [Mobile accessibility](07-mobile-accessibility.md)
