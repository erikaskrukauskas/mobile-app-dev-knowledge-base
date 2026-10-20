---
title: A dismissed screen starts clean
tags: [practices, lifecycle, navigation, state, mobile]
status: tested
updated: 2026-10-19
---

# A dismissed screen starts clean

When a person finishes a screen, or removes the app from the recent-apps list, they expect a later visit to start clean.

## Rule

Treat a completed dismissal as a new visit. Do not restore a draft they finished or a task they swiped away.

## Specify

- Which actions count as dismissal: finishing the task, swiping the app away, or force-stopping.
- Which state is cleared.
- Which state is a saved record they still expect, such as a submitted item.

## Check

Finish the screen, leave, and open it again. Transient input from the finished visit is gone. A saved record is still there. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: The user's assumption in these complete dismissal cases is that they have permanently navigated away from the screen, and if they return, they expect the screen to start from a clean state.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Save state before process death](09-save-before-process-death.md)
