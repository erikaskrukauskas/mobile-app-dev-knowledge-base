---
title: Do not share secrets over a local network socket
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# Do not share secrets over a local network socket

A port on the device can be reached by other apps. It is not a private channel.

## Rule

Talk between your own components with a mechanism that can authenticate the caller. Do not put secrets or private records on a localhost socket.

## Specify

- How components exchange data.
- What a local socket is not used for.

## Check

From another app, connect to any port the app opened. It does not return private records. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Some applications use localhost network ports for handling sensitive IPC. Don't use this approach, because these interfaces are accessible by other applications on the device.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Sharing stored data with other apps is explicit](36-exported-store-is-explicit.md)
