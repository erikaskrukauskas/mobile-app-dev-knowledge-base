---
title: Do not poll for a job the scheduler owns
tags: [practices, lifecycle, offline, mobile]
status: tested
updated: 2026-10-19
---

# Do not poll for a job the scheduler owns

Waking the app every minute to see if the network is back undoes the idle restrictions.

## Rule

Hand waiting work to the scheduler and let it run the job. The app does not keep a timer for that purpose.

## Specify

- The jobs handed off.
- The timer you do not start.

## Check

Queue waiting work and inspect wakeups during idle. There is no app heartbeat for that job. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Standard alarms and jobs are deferred into maintenance windows. Polling from the app fights that design. Schedule the work instead.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Work that can wait is scheduled](130-waiting-work-is-scheduled.md)
- [Idle alarms are rare](168-rate-limit-idle-alarms.md)
