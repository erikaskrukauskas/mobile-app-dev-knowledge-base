---
title: Show the age of offline data
tags: [practices, offline, state, screen, mobile]
status: tested
updated: 2026-10-19
---

# Show the age of offline data

A screen that shows a stored copy while the network is absent can look current when it is not.

## Rule

When the screen is showing stored data because a refresh failed or the network is absent, show that the data is stored and when it was stored.

## Specify

- Which data can be shown from the device.
- How age is shown.
- What the person can still do.

## Check

Turn the network off and open the screen. The stored data and its age are both visible. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: A user expects the UI state to remain if they temporarily switch away. Stored data shown later still needs the screen to say what they are looking at.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A network failure says what still works](41-network-failure-names-what-remains.md)
