---
title: Resume the same task
tags: [practices, lifecycle, screen, state, mobile]
status: tested
updated: 2026-10-19
---

# Resume the same task

Coming back after a call or a home press is a continuation, not a new session, unless the person dismissed the screen.

## Rule

Restore the task they left: the same screen, the same input, and the same result set when that result is still valid.

## Specify

- What 'the same task' means for this screen.
- What is refreshed because it may have gone stale.
- What is not reset.

## Check

Start a task, leave the app without dismissing it, and return. The task matches the specification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [The activity lifecycle](https://developer.android.com/guide/components/activities/activity-lifecycle). The page supports this rule: Losing the user's progress if they leave your app and return to it at a later time is a failure the lifecycle guidance calls out.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Save state before process death](09-save-before-process-death.md)
- [Show the age of offline data](27-show-data-age-when-offline.md)
