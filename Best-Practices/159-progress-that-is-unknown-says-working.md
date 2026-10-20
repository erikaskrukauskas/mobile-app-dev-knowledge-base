---
title: Unknown progress says working, not a percent
tags: [practices, screen, accessibility, mobile]
status: tested
updated: 2026-10-19
---

# Unknown progress says working, not a percent

A bar that creeps with no real measurement lies. A bar with no text is silent.

## Rule

If you know the fraction, expose it. If you do not, say the work is still going and expose that, and replace it with the result or the error when the work ends.

## Specify

- Whether the fraction is known.
- The text.
- The end states.

## Check

Run a task of unknown length with a screen reader. Working is announced. Completion replaces it. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 4.1.2: Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html). The page supports this rule: Values and changes to values need to be available to assistive technologies. A loading indicator is one of those values.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A loading screen says it is waiting](80-loading-state-says-waiting.md)
