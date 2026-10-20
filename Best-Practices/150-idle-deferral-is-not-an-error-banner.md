---
title: An idle deferral is not an error banner
tags: [practices, error, offline, screen, mobile]
status: tested
updated: 2026-10-19
---

# An idle deferral is not an error banner

The person did nothing wrong when the system waits to sync.

## Rule

Do not show a failure banner because a background job has not run during idle. Show age of data if they are looking at stored data. Reserve the error banner for a call they just made that failed.

## Specify

- The quiet waiting state.
- The error state for an action they took.
- The age label.

## Check

Idle the device, then open the app. There is no error banner for the deferred job. Pull to refresh with the network unusable and the error state appears. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Jobs and syncs are deferred on purpose during idle. That deferral is system behavior, not a failed action by the person.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A network failure says what still works](41-network-failure-names-what-remains.md)
- [Show the age of offline data](27-show-data-age-when-offline.md)
