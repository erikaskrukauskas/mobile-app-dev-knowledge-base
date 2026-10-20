---
title: Honor reduced motion
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# Honor reduced motion

Motion that explains a change can also make a person sick or hide the change.

## Rule

When the platform's reduced-motion setting is on, replace nonessential animation with a simple change. Keep motion that is the only indication of state, and also expose that state in text.

## Specify

- Which animations are essential.
- What replaces the others.
- The setting the check uses.

## Check

Turn on reduced motion and move between screens. Nonessential animation is gone, and the state is still understandable. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [WCAG 2 Overview](https://www.w3.org/WAI/standards-guidelines/wcag/). The page supports this rule: WCAG organizes requirements under perceivable, operable, understandable, and robust. A motion setting is an operable and perceivable constraint. Confirm the current platform setting before you name the API.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Mobile accessibility](07-mobile-accessibility.md)
