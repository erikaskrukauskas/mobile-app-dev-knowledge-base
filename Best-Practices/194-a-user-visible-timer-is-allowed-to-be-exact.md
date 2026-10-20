---
title: A timer they set is allowed to be exact
tags: [practices, screen, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# A timer they set is allowed to be exact

A cooking timer or a reminder they just created is a promise about a clock time.

## Rule

Fire a timer they set at the time they set, and show it. Do not apply the idle-wait rule to that promise. Do not use this path for work they did not ask to see.

## Specify

- Which timers are theirs.
- What appears when one fires.
- Which jobs still wait.

## Check

Set a short timer, lock the device, and wait. It fires at the promised time. A background sync during the same wait may not. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Alarm-clock style alarms continue to fire while idle, and the system leaves idle shortly before they fire. Other alarms are deferred.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A silent heartbeat is not a user alarm](146-a-silent-heartbeat-is-not-an-alarm.md)
