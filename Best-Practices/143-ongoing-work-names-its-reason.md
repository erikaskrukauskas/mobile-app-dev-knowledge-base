---
title: Ongoing work names why it is allowed to continue
tags: [practices, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Ongoing work names why it is allowed to continue

Platforms ask you to declare the kind of ongoing work. The reason is also how you know when to stop.

## Rule

Name the reason the work continues: playback, an activity they started, a transfer they are watching. Stop the work when that reason ends. Do not reuse the reason for a second, hidden job.

## Specify

- The reason.
- The stop condition.
- The visible status.

## Check

Start the named task and finish it. The status ends when the reason ends. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: The foreground-service guidance covers service types, launching, stopping, and restrictions on starting that work from the background.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Ongoing work the person is not watching is still visible](109-ongoing-work-is-visible.md)
- [The person can stop ongoing work](110-person-can-stop-ongoing-work.md)
