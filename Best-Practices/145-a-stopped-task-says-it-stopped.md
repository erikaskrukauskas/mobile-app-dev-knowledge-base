---
title: If the system stops a long task, say so
tags: [practices, lifecycle, error, screen, mobile]
status: tested
updated: 2026-10-19
---

# If the system stops a long task, say so

Some platforms limit how long ongoing work may run. The person should not think it is still going.

## Rule

When a long task is stopped by the system or by a time limit, update the visible status and the screen. Say whether a partial result was kept.

## Specify

- The time or condition that stops it.
- The message.
- What was saved.

## Check

Run the task until the stop condition. The status and the screen both show that it stopped. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: The foreground-service guidance includes timeout behavior. A task the system stops should not keep claiming it is running.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The person can stop ongoing work](110-person-can-stop-ongoing-work.md)
