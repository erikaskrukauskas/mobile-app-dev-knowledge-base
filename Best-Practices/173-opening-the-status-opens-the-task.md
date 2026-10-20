---
title: Opening the ongoing status opens that task
tags: [practices, navigation, screen, mobile]
status: tested
updated: 2026-10-19
---

# Opening the ongoing status opens that task

Tapping the notice for a recording or a download should land on that task, not on the home screen.

## Rule

The ongoing status opens the screen for that task. If the task already finished, open the result or the fallback, not a blank start.

## Specify

- The screen it opens.
- The fallback if the task is gone.

## Check

Tap the status during the task and after it has finished. Both landings match the specification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: A foreground notification names the current task, such as the song playing or the distance traveled. Opening it should return to that task.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A notification opens the screen that holds the state](85-notification-opens-the-state.md)
