---
title: Back returns to the previous place
tags: [practices, navigation, screen, mobile]
status: tested
updated: 2026-10-19
---

# Back returns to the previous place

Back means the person returns to the place they came from, in an order they can predict.

## Rule

Each forward move has a back move to a known screen. Back does not jump to an unrelated section or exit when a previous screen still exists.

## Specify

- The previous screen for each forward move.
- When back leaves the app, because there is no previous screen.
- What state the previous screen shows.

## Check

Open three screens in order and go back twice. The screens appear in reverse order. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Navigation](https://developer.android.com/guide/navigation). The page supports this rule: Navigation refers to the interactions that let users navigate across, into, and back out from the different pieces of content within your app.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Say when up and back differ](23-up-and-back.md)
- [Back does not silently drop unsaved input](24-back-keeps-unsaved-input.md)
