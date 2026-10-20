---
title: A decorative image is skipped by assistive technology
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A decorative image is skipped by assistive technology

A flourish that is announced as an image makes the screen longer without adding meaning.

## Rule

Hide decorative and purely formatting images from assistive technology. Do not give them a name like image or icon.

## Specify

- Which images are decorative.
- How they are hidden.

## Check

Move through the screen with a screen reader. Decorative images are not announced. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 1.1.1: Non-text Content](https://www.w3.org/WAI/WCAG22/Understanding/non-text-content.html). The page supports this rule: If non-text content is pure decoration, visual formatting, or not presented to users, implement it so assistive technology can ignore it.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A meaningful image has equivalent text](135-a-meaningful-image-has-an-equivalent-text.md)
