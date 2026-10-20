---
title: Work that can wait is scheduled
tags: [practices, offline, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Work that can wait is scheduled

Starting a large job the moment any network appears fights the radio and the battery limits.

## Rule

Schedule work that can wait so it runs when a suitable network exists. Do not spin a timer in the app to poll for that network.

## Specify

- Which jobs wait.
- The condition they wait for.
- What the person sees meanwhile.

## Check

Queue a waiting download with no suitable network, then provide one. The download runs without a polling loop in the foreground. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: If your app needs to schedule tasks for when the device next has connectivity or is on an unmetered network, schedule that work rather than polling connectivity.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A large transfer respects a metered network](128-large-transfer-respects-a-metered-network.md)
