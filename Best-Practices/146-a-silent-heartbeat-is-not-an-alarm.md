---
title: A silent heartbeat is not a user alarm
tags: [practices, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# A silent heartbeat is not a user alarm

An alarm the person created, such as a wake-up time, is allowed to fire. A timer whose only job is to wake the app is not that alarm.

## Rule

Reserve exact alarms that fire while the device is idle for events the person asked to be woken for. A sync heartbeat waits for a maintenance window.

## Specify

- The alarms the person set.
- The work that waits.

## Check

Set a user alarm and a background refresh. The alarm can fire while idle. The refresh may wait. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Alarms set as an alarm-clock style alarm continue to fire, and the system exits idle shortly before they fire. Allow-while-idle alarms are rate limited, on the order of once per nine minutes per app.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Background sync may wait until the device is idle-awake](112-background-sync-may-wait.md)
