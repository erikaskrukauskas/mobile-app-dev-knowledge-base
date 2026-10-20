---
title: Two ongoing tasks have two statuses
tags: [practices, screen, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Two ongoing tasks have two statuses

One generic ongoing notice for two different jobs hides which one is running and which stop button does what.

## Rule

Give each ongoing task its own status, its own stop, and its own open target. Do not merge unrelated tasks into one notice.

## Specify

- The tasks.
- The status for each.

## Check

Start two tasks. Two statuses appear. Stopping one leaves the other running. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: Each foreground task is noticeable on its own, with a notification that makes the person aware of that task.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Ongoing work the person is not watching is still visible](109-ongoing-work-is-visible.md)
