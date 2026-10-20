---
title: Say which network facts the screen uses
tags: [practices, offline, screen, mobile]
status: tested
updated: 2026-10-19
---

# Say which network facts the screen uses

Connected, metered, captive, and validated are different facts. A screen that says offline for all of them hides the choice.

## Rule

Write down which facts change this screen: none, metered, captive, or no route to the server. Use a different message only where the person can do something different.

## Specify

- The facts.
- The message for each fact you distinguish.
- The facts you deliberately collapse into one message.

## Check

Produce each fact you listed and read the message. It matches the specification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: Network capabilities expose transports, metering, and captive-portal state. The screen should use the facts that change what the person can do.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A captive portal is not a reachable server](127-captive-portal-is-not-your-server.md)
- [A large transfer respects a metered network](128-large-transfer-respects-a-metered-network.md)
