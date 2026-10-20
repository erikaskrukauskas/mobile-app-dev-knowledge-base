---
title: A custom authority is named, not global
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# A custom authority is named, not global

Trusting a company or self-signed authority for one host should not make that authority valid for every host.

## Rule

Scope a custom authority to the hosts that need it. Other hosts keep the ordinary public set.

## Specify

- The hosts.
- The authority.
- A host that must not trust it.

## Check

Use the custom authority against a different host. That call fails. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Network security configuration](https://developer.android.com/privacy-and-security/security-config). The page supports this rule: You can customize trust per domain. A custom trust anchor is for hosts that need it, such as an internal authority.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A sensitive call trusts a named set of authorities](126-sensitive-calls-trust-a-named-set.md)
