---
title: A late callback does not update a screen that is gone
tags: [practices, lifecycle, error, mobile]
status: tested
updated: 2026-10-19
---

# A late callback does not update a screen that is gone

A response can arrive after the person has left the screen or after the process has a new screen in its place.

## Rule

Ignore or reroute a result if the screen that asked for it is gone. Do not write that result over a newer edit, and do not navigate a screen they already left.

## Specify

- How you know the screen is gone.
- Where a still-useful result is stored.
- What is discarded.

## Check

Start a request, leave the screen, and deliver the response. The screen they are on now does not jump, and a newer draft is unchanged. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: Connectivity and requests change over time. A one-shot check or a late callback is not permission to redraw a screen that has already moved on.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Do not start a new flow in the background](14-no-new-flow-from-background.md)
