---
title: Cleartext network access stays off
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# Cleartext network access stays off

An unencrypted call is easy to add by accident when a URL changes.

## Rule

Keep cleartext off for the app. If one named host must use it, opt in for that host only and say why. Do not turn cleartext on for every host.

## Specify

- The hosts that are protected.
- Any host that is cleartext, and why.
- What the screen does when a protected call fails.

## Check

Point a request at an unencrypted URL that is not on the exception list. The call does not succeed, and secrets are not sent. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Network security configuration](https://developer.android.com/privacy-and-security/security-config). The page supports this rule: Cleartext traffic opt-out protects apps from accidental usage of unencrypted traffic. Starting with Android 9, cleartext is disabled by default. Opting in for any domain should be avoided whenever possible.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Use protected transport on networks you do not control](54-https-on-networks-you-do-not-control.md)
