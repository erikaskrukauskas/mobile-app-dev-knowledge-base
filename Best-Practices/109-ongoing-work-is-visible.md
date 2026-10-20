---
title: Ongoing work the person is not watching is still visible
tags: [practices, lifecycle, screen, mobile]
status: tested
updated: 2026-10-19
---

# Ongoing work the person is not watching is still visible

Work that continues while the person is in another app has to be obvious. A hidden task that holds the radio or the microphone is not.

## Rule

If work must continue while the app is not on screen, show a status the person can see, such as a notification that names the task. If the work is too quiet to deserve that status, defer it instead of hiding it.

## Specify

- The task that continues.
- The visible status.
- The work that is deferred because it is not worth a visible status.

## Check

Start the task and leave the app. The status is visible. Stop the task and the status is gone. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: Foreground services show a status bar notification, to make users aware that your app is performing a task in the foreground and is consuming system resources. If the action is of low enough importance that you want to use a minimum-priority notification, use a different background option.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Release work when the app is not visible](12-release-work-when-backgrounded.md)
