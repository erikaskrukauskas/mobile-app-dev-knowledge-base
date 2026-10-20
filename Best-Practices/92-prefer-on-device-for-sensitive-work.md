---
title: Do sensitive work on the device when the server does not need the data
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# Do sensitive work on the device when the server does not need the data

Sending personal data to a server creates a copy the screen may not need.

## Rule

If the operation can be done on the device, do it there and avoid the transmission. Send the data only when the specification says a server must see it.

## Specify

- Which operations stay on the device.
- Which payloads are sent, and why.

## Check

Run the on-device operation and confirm no request carries the personal payload. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: If your app requires access to sensitive data, evaluate whether you need to transmit it to a server or if you can run the operation on the client.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Keep as little personal data on the device as the screen needs](56-minimize-personal-data-on-the-device.md)
