---
title: An unverified link is not the caller's identity
tags: [practices, navigation, security, mobile]
status: tested
updated: 2026-10-19
---

# An unverified link is not the caller's identity

A custom scheme or an unverified web link can be claimed by more than one app, and the system may ask the person to choose.

## Rule

Do not treat the arrival of a link as proof of who sent it or as permission to perform a sensitive action. Show the destination, and require the same confirmation a person would see inside the app.

## Specify

- Which links open a screen only.
- Which actions still need an in-app confirmation.
- What the person sees if the system asks them to pick an app.

## Check

Open a sensitive action from an unverified link. The action does not run until the in-app confirmation. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [About deep links](https://developer.android.com/training/app-links). The page supports this rule: Deep links are subject to the system disambiguation dialog.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Prefer a verified association for your own links](21-verified-app-link.md)
- [Mobile application security](06-mobile-application-security.md)
