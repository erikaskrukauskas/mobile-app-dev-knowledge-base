---
title: Idle alarms are rare
tags: [practices, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Idle alarms are rare

A loop of exact alarms while the device is idle is a battery bug, and the platform will coalesce it anyway.

## Rule

Do not schedule a stream of exact idle alarms. One rare alarm for a real event is the shape that fits. Everything else is scheduled work.

## Specify

- The events that may use an idle alarm.
- The maximum rate you will schedule.
- The work that uses the scheduler instead.

## Check

Inspect scheduled alarms during idle. They match the rare list, not a heartbeat. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Allow-while-idle alarms cannot fire more than once per nine minutes per app. Standard alarms are deferred to the next maintenance window.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A silent heartbeat is not a user alarm](146-a-silent-heartbeat-is-not-an-alarm.md)
