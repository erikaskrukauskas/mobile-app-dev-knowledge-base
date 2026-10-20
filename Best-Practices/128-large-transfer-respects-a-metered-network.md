---
title: A large transfer respects a metered network
tags: [practices, offline, screen, mobile]
status: tested
updated: 2026-10-19
---

# A large transfer respects a metered network

A photo backup or a dataset download on a metered link can cost the person money.

## Rule

A large transfer waits for an unmetered network, or it asks first. A small, time-critical request may proceed. Say which transfers are large.

## Specify

- What counts as large.
- The ask, or the wait.
- How they start it now anyway.

## Check

Start a large transfer on a metered network. It waits or asks. It does not upload the payload silently. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: Network capabilities include whether the network is metered. Schedule work that can wait, such as a background download, for an unmetered network.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Background sync may wait until the device is idle-awake](112-background-sync-may-wait.md)
