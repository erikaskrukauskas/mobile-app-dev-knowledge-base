---
title: Returning from another app restores the screen
tags: [practices, lifecycle, navigation, state, mobile]
status: tested
updated: 2026-10-19
---

# Returning from another app restores the screen

A share sheet, a browser, or a payment app sends the person away and then back.

## Rule

When they return, the screen shows the task they left and the result of the outside step if one came back. It does not restart at the root.

## Specify

- Which outside steps the screen can start.
- What result they may bring back.
- What the screen shows if they cancel outside.

## Check

Start an outside step, complete it, and cancel it in a second run. Both returns match the specification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [The activity lifecycle](https://developer.android.com/guide/components/activities/activity-lifecycle). The page supports this rule: Losing the user's progress if they leave your app and return to it at a later time is a failure mode the lifecycle guidance names.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Resume the same task](13-resume-the-same-task.md)
