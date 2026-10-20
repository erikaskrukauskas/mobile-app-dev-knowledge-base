---
title: Do not use a phone identifier as the account id
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# Do not use a phone identifier as the account id

A phone number or a hardware identifier is tied to the person and to the device. It is a poor account key and a privacy leak.

## Rule

Create an identifier for the account or the install. Do not key records by the phone number, the device id, or a similar hardware identifier.

## Specify

- The identifier the app creates.
- What it is not.
- Where it is stored.

## Check

Inspect the local store and the outbound calls from a fresh install. The account key is the created identifier. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: If a Globally Unique Identifier is required, create a large, unique number and store it. Don't use phone identifiers such as the phone number or IMEI.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Keep as little personal data on the device as the screen needs](56-minimize-personal-data-on-the-device.md)
