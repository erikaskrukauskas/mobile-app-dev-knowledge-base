---
title: Do not stay awake just to avoid being treated as idle
tags: [practices, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Do not stay awake just to avoid being treated as idle

Holding a visible ongoing task so the system will not treat the app as idle drains the battery for no task the person asked for.

## Rule

Start ongoing visible work only for a task the person expects to continue immediately, such as playback or an activity they started. Do not start it so the app will keep syncing in the background.

## Specify

- The tasks allowed to stay active.
- The sync that must wait instead.

## Check

Leave the app idle with no playback and no active recording. It does not post an ongoing status merely to keep syncing. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Don't start a foreground service just to prevent the system from determining that your app is idle. Only use a foreground service for tasks the user expects the system to execute immediately or without interruption.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Ongoing work the person is not watching is still visible](109-ongoing-work-is-visible.md)
- [Background sync may wait until the device is idle-awake](112-background-sync-may-wait.md)
