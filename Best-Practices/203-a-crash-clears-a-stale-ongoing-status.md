---
title: A crash does not leave a lying status
tags: [practices, error, lifecycle, screen, mobile]
status: tested
updated: 2026-10-19
---

# A crash does not leave a lying status

If the process dies, a status that still says live is worse than no status.

## Rule

When the process dies or the task cannot continue, the ongoing status is removed or replaced with a failure the person can open. It does not keep saying the task is healthy.

## Specify

- Who clears the status.
- What they see if they tap a failure notice.

## Check

Kill the process during the task. The healthy ongoing status does not remain. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: The notification is true only while the task is running. A dead process is not a running foreground task.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A finished task clears its status](175-a-finished-task-clears-its-status.md)
