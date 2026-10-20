---
title: An offline command applies once
tags: [practices, offline, state, error, mobile]
status: tested
updated: 2026-10-19
---

# An offline command applies once

A command queued while offline can be sent twice when the network returns, or sent again after the app restarts.

## Rule

Replaying the queue applies each command once. A second delivery of the same command does not create a second effect. The general rule for idempotent commands lives in the application-development knowledge base. This page is the mobile queue.

## Specify

- What is queued.
- The identity used to recognize a replay.
- What the person sees while the command is waiting, and if it fails.

## Check

Create a command offline, restore the network, and restart the app before the queue finishes. The effect exists once. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: Persistent storage is what survives process death. A queue that lives only in memory can run twice or not at all after the process dies.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Show the age of offline data](27-show-data-age-when-offline.md)
