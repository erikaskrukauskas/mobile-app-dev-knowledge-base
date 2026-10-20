---
title: A refresh on open is honest about age
tags: [practices, offline, screen, mobile]
status: tested
updated: 2026-10-19
---

# A refresh on open is honest about age

Opening the app is when deferred work may finally run. The first paint might still be the stored copy.

## Rule

Show the stored copy and its age immediately, then update when the refresh returns. Do not hold the first screen on a blank loader for a sync that idle was allowed to delay.

## Specify

- What the first paint shows.
- What the refresh replaces.
- The failure state if the refresh fails.

## Check

Open the app on a stored copy. The copy and its age appear before the refresh finishes. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Deferred syncs run when the device or app wakes. Until that refresh returns, the UI the person already had is the stored one.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Show the age of offline data](27-show-data-age-when-offline.md)
- [A loading screen says it is waiting](80-loading-state-says-waiting.md)
