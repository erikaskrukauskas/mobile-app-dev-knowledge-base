---
title: Do not chain urgent wakes
tags: [practices, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Do not chain urgent wakes

One urgent alert that fetches more data and then sends another urgent message keeps the device awake.

## Rule

An urgent message stands alone. Further sync uses ordinary priority. The person can open the app for the rest.

## Specify

- The urgent messages.
- The follow-up work and its priority.

## Check

Deliver one urgent alert while idle and confirm it does not schedule a second urgent wake. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: High priority is for messages that result in a notification, and the payload should be sufficient so more network access is unnecessary.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A push that alerts carries its text](147-a-push-carries-its-text.md)
