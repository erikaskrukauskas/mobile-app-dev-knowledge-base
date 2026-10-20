---
title: A captive portal is not a reachable server
tags: [practices, offline, error, screen, mobile]
status: tested
updated: 2026-10-19
---

# A captive portal is not a reachable server

The phone can be joined to a network and still be stuck on a sign-in page. That is not a successful call to your server, and it is not proof the person has no account.

## Rule

When the network is captive or otherwise unable to reach your server, say that the connection is not usable yet. Keep local data on screen. Do not wipe it and do not treat the portal as a response from your API.

## Specify

- How the screen describes this state.
- What remains usable.
- What happens after the network becomes usable.

## Check

Join a captive network and open the screen. The message is not the empty-account message, and local work remains. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: Network capabilities can say whether a network is behind a captive portal. A Network object also stops being usable when that network disconnects.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A network failure says what still works](41-network-failure-names-what-remains.md)
