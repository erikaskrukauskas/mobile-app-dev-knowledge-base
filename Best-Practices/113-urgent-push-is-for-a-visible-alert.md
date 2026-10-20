---
title: An urgent push is for an alert the person will see
tags: [practices, screen, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# An urgent push is for an alert the person will see

Waking the device for a message that only refreshes a cache spends the battery and trains them to ignore alerts.

## Rule

Use an urgent, high-priority delivery only when it produces an alert the person can see. A silent refresh uses an ordinary delivery that is allowed to wait.

## Specify

- Which messages become alerts.
- Which messages only refresh data.
- The alert text, which is in the message rather than fetched afterward when the alert must be immediate.

## Check

Send one alert message and one silent refresh while the device is idle. The alert appears. The refresh may wait. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Only use high priority for messages that result in a notification. Provide sufficient information within the initial message payload, so subsequent network access is unnecessary.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A notification opens the screen that holds the state](85-notification-opens-the-state.md)
