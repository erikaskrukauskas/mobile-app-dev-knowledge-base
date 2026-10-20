---
title: A deep link has a fallback screen
tags: [practices, navigation, screen, error, mobile]
status: tested
updated: 2026-10-19
---

# A deep link has a fallback screen

A link can name a screen or a record that is gone, private, or not loaded yet.

## Rule

Opening a link either shows the named content or a defined fallback. It does not show a blank stack or a crash.

## Specify

- The content the link may open.
- The fallback when the content is missing, unauthorized, or offline.
- Whether the fallback still offers a way home.

## Check

Open a link to a deleted record and a link to a valid one. Each matches the specification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [About deep links](https://developer.android.com/training/app-links). The page supports this rule: Android deep links let you bring users directly into your app content from links they have tapped.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [An unverified link is not the caller's identity](20-unverified-link-is-not-identity.md)
- [A failed restore opens a safe screen](15-safe-screen-when-restore-fails.md)
