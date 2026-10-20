---
title: A tunnel is not proof your server answered
tags: [practices, security, offline, mobile]
status: tested
updated: 2026-10-19
---

# A tunnel is not proof your server answered

A VPN or a private DNS setting can be up while your server is down, or the tunnel can be the thing that failed.

## Rule

Treat those as network conditions. Success is still a response from your server. A tunnel failure uses the same unreachable state, not a blank error.

## Specify

- The unreachable message.
- That it does not claim the account is gone.

## Check

Block the server while the device still shows a connected transport. The screen shows unreachable and keeps local data. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: Capabilities describe transports and whether the network can actually carry the traffic you care about. Presence of a transport is not the response.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A connected network is not a successful response](129-a-network-object-is-not-success.md)
