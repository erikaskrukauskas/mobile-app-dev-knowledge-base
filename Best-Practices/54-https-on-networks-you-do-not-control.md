---
title: Use protected transport on networks you do not control
tags: [practices, security, offline, mobile]
status: tested
updated: 2026-10-19
---

# Use protected transport on networks you do not control

Phones join networks the person does not control. A cleartext call on that network is readable.

## Rule

Send sensitive data only over a protected transport. Do not trust a response that arrived in cleartext.

## Specify

- Which calls carry sensitive data.
- The transport they use.
- What the screen does if the protected connection fails.

## Check

Attempt the call on a network that blocks or strips the protected transport. The app does not fall back to cleartext for the sensitive payload, and the screen says the connection failed. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Use HTTPS over HTTP anywhere that HTTPS is supported on the server, because mobile devices frequently connect on networks that aren't secured, such as public Wi-Fi hotspots.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A network failure says what still works](41-network-failure-names-what-remains.md)
