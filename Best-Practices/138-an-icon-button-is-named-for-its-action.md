---
title: An icon button is named for its action
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# An icon button is named for its action

A button whose accessible name is the image file name, or button, does not say what will happen.

## Rule

Name an icon-only button with the action, such as Delete or Close. The name matches the purpose, not the asset name.

## Specify

- Each icon-only control.
- Its name.

## Check

Focus each icon button with a screen reader. The action is spoken. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 1.1.1: Non-text Content](https://www.w3.org/WAI/WCAG22/Understanding/non-text-content.html). The page supports this rule: If non-text content is a control or accepts input, it has a name that describes its purpose.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The accessible name matches the visible label](70-label-matches-visible-text.md)
