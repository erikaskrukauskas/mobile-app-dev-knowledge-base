---
title: A finished task clears its status
tags: [practices, screen, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# A finished task clears its status

A notice that still says recording after they pressed stop teaches them not to trust the status.

## Rule

When the task completes, fails, or is stopped, remove or update the ongoing status immediately so it matches the real state.

## Specify

- The moment it clears.
- Any completion notice, which is a separate alert decision.

## Check

Finish the task. The ongoing status is gone. The in-app screen shows the result. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: The notification exists while the foreground task is running. Stopping the service is part of the same guidance, so the notice must not outlive the task.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A badge matches the unread state](87-badge-matches-unread-state.md)
