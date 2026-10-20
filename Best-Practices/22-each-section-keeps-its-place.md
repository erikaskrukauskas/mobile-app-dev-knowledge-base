---
title: Each top-level section keeps its place
tags: [practices, navigation, state, mobile]
status: tested
updated: 2026-10-19
---

# Each top-level section keeps its place

Switching top-level sections and coming back should show the place the person left, not the root of that section every time.

## Rule

Give each top-level section its own place in the stack. Changing sections does not destroy the other section's screen unless the person finished that task.

## Specify

- The top-level sections.
- What each one restores.
- What a finished task clears.

## Check

Open a detail in one section, switch to another section, and switch back. The detail is still there. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Navigation](https://developer.android.com/guide/navigation). The page supports this rule: The navigation guidance treats back and up, and the destinations in a graph, as a structure the person can move through and return through.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Back returns to the previous place](17-back-returns-to-previous.md)
- [A dismissed screen starts clean](10-clean-start-after-dismissal.md)
