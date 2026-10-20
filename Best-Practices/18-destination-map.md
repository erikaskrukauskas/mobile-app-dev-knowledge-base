---
title: Name the destinations and how they connect
tags: [practices, navigation, screen, mobile]
status: tested
updated: 2026-10-19
---

# Name the destinations and how they connect

A mobile client needs an explicit list of screens and the moves between them. A pile of buttons is not that list.

## Rule

Write the destinations and the connections a person can take, including back. The same map applies whether the screens are native views or a cross-platform toolkit.

## Specify

- The destinations.
- The connections, including which ones are forward, back, or a replacement.
- The data each destination needs in order to open.

## Check

Walk every connection in the map on a device. Each one opens the named destination, and back follows the map. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Navigation](https://developer.android.com/guide/navigation). The page supports this rule: Whether you are using Compose, views, or a custom UI framework, these concepts always apply when implementing navigation.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Back returns to the previous place](17-back-returns-to-previous.md)
- [Compare before choosing](03-compare-before-choosing.md)
