---
title: Background sync may wait until the device is idle-awake
tags: [practices, offline, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Background sync may wait until the device is idle-awake

A phone that is still, unplugged, and dark defers network and jobs. A sync started then does not have to finish then.

## Rule

Treat a deferred sync as waiting, not as a failure the person must fix. Show fresh data when they open the app or when the waiting work runs. Do not surface an error solely because the system deferred the job.

## Specify

- Which syncs may wait.
- What the screen shows if they open the app before the sync runs.
- What is not deferred because they are waiting on it now.

## Check

Leave the device idle, then open the app. Local data is still usable, and a deferred sync is not presented as a broken account. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Doze defers background CPU and network activity, and defers jobs, syncs, and standard alarms, until a maintenance window or until the person wakes the device.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Show the age of offline data](27-show-data-age-when-offline.md)
- [A network failure says what still works](41-network-failure-names-what-remains.md)
