---
title: Prefer a verified association for your own links
tags: [practices, navigation, security, mobile]
status: tested
updated: 2026-10-19
---

# Prefer a verified association for your own links

A link to your own site should open your app without asking the person to pick from a list, once the association is verified.

## Rule

When the product owns the web address, use the platform's verified association so the link opens the app directly. Confirm the current setup steps before relying on them. An unverified custom scheme stays on [An unverified link is not the caller's identity](20-unverified-link-is-not-identity.md).

## Specify

- The addresses the app claims.
- The fallback when verification is absent.
- The screen each address opens.

## Check

Tap a verified link to a record you own. The app opens on that record without a chooser. Tap an unverified scheme and confirm it does not skip confirmation for a sensitive action. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [About deep links](https://developer.android.com/training/app-links). The page supports this rule: After they are verified, deep links to your website can immediately open corresponding content in your app, without requiring the user to select your app from a disambiguation dialog.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [An unverified link is not the caller's identity](20-unverified-link-is-not-identity.md)
- [A deep link has a fallback screen](19-deep-link-fallback.md)
