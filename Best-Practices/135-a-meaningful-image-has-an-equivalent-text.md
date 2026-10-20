---
title: A meaningful image has equivalent text
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A meaningful image has equivalent text

A photo, chart, or icon that carries information needs text that carries the same information, not the file name.

## Rule

Write a text alternative that serves the same purpose as the image. Image or chart alone is not that text. A control that is an image uses a name that states the action.

## Specify

- The images that carry meaning.
- The text for each.
- The images that are decorative and therefore skipped.

## Check

Open the screen with images unloaded, or with a screen reader. The information and the actions are still available as text. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 1.1.1: Non-text Content](https://www.w3.org/WAI/WCAG22/Understanding/non-text-content.html). The page supports this rule: All non-text content that is presented to the user has a text alternative that serves the equivalent purpose, except listed cases such as decoration.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A status icon also has text](72-status-icons-have-text.md)
- [A decorative image is skipped by assistive technology](134-decorative-images-are-skipped.md)
