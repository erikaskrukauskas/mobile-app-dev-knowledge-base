---
title: A third-party component gets no unexplained personal data
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# A third-party component gets no unexplained personal data

An analytics, advertising, or support library runs inside the app and can receive what you pass it.

## Rule

Do not pass personal data to a component when you cannot say why it needs that data. Leave the field out.

## Specify

- Which components receive data.
- The fields each one gets.
- The fields they do not get.

## Check

Exercise the screen and capture what the component receives. Unexplained personal fields are absent. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: If you don't know why a component or service requires personal information, don't provide it.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Keep as little personal data on the device as the screen needs](56-minimize-personal-data-on-the-device.md)
