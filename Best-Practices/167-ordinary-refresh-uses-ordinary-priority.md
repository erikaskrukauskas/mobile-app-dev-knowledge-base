---
title: An ordinary refresh uses ordinary priority
tags: [practices, offline, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# An ordinary refresh uses ordinary priority

Marking every sync urgent makes urgent meaningless and wakes the device all day.

## Rule

Use ordinary delivery for cache refresh and sync. Those may arrive during a maintenance window or when the person opens the app.

## Specify

- The ordinary messages.
- The urgent ones, which are only visible alerts.

## Check

Send an ordinary refresh while idle. It may wait. It does not light the screen. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: For messages that don't result in notifications, such as keeping content up to date or initiating a sync, use normal priority. In idle mode they are delivered during maintenance windows or when the user wakes the device.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [An urgent push is for an alert the person will see](113-urgent-push-is-for-a-visible-alert.md)
