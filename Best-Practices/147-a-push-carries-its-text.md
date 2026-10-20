---
title: A push that alerts carries its text
tags: [practices, screen, offline, mobile]
status: tested
updated: 2026-10-19
---

# A push that alerts carries its text

Waking the device and then fetching the message body forces another network call at the worst time.

## Rule

Put the alert text in the payload. Fetch the rest when the person opens the app. A silent update does not use an urgent wake.

## Specify

- What is in the payload.
- What is loaded on open.

## Check

Deliver an alert while idle. The text appears without a second fetch. Open the app and the rest can load then. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Provide sufficient information within the initial message payload, so subsequent network access is unnecessary.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [An urgent push is for an alert the person will see](113-urgent-push-is-for-a-visible-alert.md)
