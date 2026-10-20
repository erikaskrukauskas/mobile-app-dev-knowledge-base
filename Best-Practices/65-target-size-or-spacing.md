---
title: Make touch targets large enough or far enough apart
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# Make touch targets large enough or far enough apart

Small controls placed against each other are easy to hit by mistake.

## Rule

Give each control at least a 24 by 24 CSS pixel target, or space undersized targets so a 24 pixel circle around each does not overlap the next. Confirm any stricter platform minimum before you rely on it. Exceptions in the criterion, such as inline links in a sentence, stay exceptions.

## Specify

- The minimum you are applying.
- Any control that uses the spacing exception.
- Any control that uses an inline exception.

## Check

On a phone, attempt the adjacent controls. The wrong neighbor does not activate when the person aims at the named control. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 2.5.8: Target Size (Minimum)](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html). The page supports this rule: The size of the target for pointer inputs is at least 24 by 24 CSS pixels, with listed exceptions including spacing, an equivalent larger control, and inline text.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Mobile accessibility](07-mobile-accessibility.md)
