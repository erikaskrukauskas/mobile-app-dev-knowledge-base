---
title: Waiting work may run when the device is charging
tags: [practices, offline, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Waiting work may run when the device is charging

Plugging in is one of the moments the system lets waiting jobs run. The person should not have to babysit that.

## Rule

Let scheduled work run when the device leaves idle because it is charging or awake. Do not require them to open the app for a job you already said could wait, and do not notify them that the job ran unless they asked for an alert.

## Specify

- Which jobs run quietly when charging.
- Which results deserve an alert.

## Check

Queue a waiting job, charge the device, and leave the app closed. The job can complete without an alert. The result is there when they open the app. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: When the user connects a charger, the system exits Doze. When the device is plugged in, apps in standby are released to run pending jobs.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Work that can wait is scheduled](130-waiting-work-is-scheduled.md)
