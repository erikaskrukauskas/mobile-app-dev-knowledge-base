---
title: Test offline with the network off
tags: [practices, testing, offline, mobile]
status: tested
updated: 2026-10-19
---

# Test offline with the network off

A mock that returns an error is not the same as a phone with no network.

## Rule

Run the offline check with the device network disabled. Confirm stored data, queued commands, and the failure message.

## Specify

- How the network is disabled.
- What the screen must show.
- What happens when the network returns.

## Check

Disable the network, use the screen, then enable it. The specification for offline and for replay both hold. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Test apps on Android](https://developer.android.com/training/testing). The page supports this rule: Testing is how you verify functional behavior before release. Offline behavior is functional behavior of a mobile client.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Show the age of offline data](27-show-data-age-when-offline.md)
- [An offline command applies once](29-offline-command-applies-once.md)
