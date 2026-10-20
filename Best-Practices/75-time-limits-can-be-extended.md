---
title: A time limit can be extended or is explained
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# A time limit can be extended or is explained

A code entry or a session that expires while a person is still working fails people who need more time.

## Rule

If the screen will time out an input, let the person extend it, or say how long they have before they start. Do not clear what they typed without a warning.

## Specify

- Which screens time out.
- How they warn or extend.
- What is kept when time runs out.

## Check

Start the timed input and wait. The warning or the extension matches the specification, and typed input is not silently cleared. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [WCAG 2 Overview](https://www.w3.org/WAI/standards-guidelines/wcag/). The page supports this rule: WCAG includes operable requirements for time limits. Confirm the current success criterion before claiming a specific timeout behavior.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Back does not silently drop unsaved input](24-back-keeps-unsaved-input.md)
