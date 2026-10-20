---
title: A connected network is not a successful response
tags: [practices, offline, error, mobile]
status: tested
updated: 2026-10-19
---

# A connected network is not a successful response

Seeing that Wi-Fi is associated does not mean your server answered.

## Rule

Decide success from the response, not from the existence of a network. Update the screen when connectivity actually changes, instead of checking once at startup and polling afterward.

## Specify

- What the screen treats as success.
- What it treats as no usable connection.
- That it listens for changes rather than polling.

## Check

Start on a network that cannot reach the server. The screen shows the failure state, not a spinner that never ends and not a fake success. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: Synchronous connectivity checks do not tell you about later changes and do not by themselves update the UI. Register for the changes you care about instead of polling.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A captive portal is not a reachable server](127-captive-portal-is-not-your-server.md)
