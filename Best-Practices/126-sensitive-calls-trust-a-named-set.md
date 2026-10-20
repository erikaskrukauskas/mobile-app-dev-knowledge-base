---
title: A sensitive call trusts a named set of authorities
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# A sensitive call trusts a named set of authorities

Trusting every certificate on the device includes ones the person, or someone with the device, added.

## Rule

For sensitive connections, trust an explicit set of authorities. Do not inherit every user-added authority for those hosts.

## Specify

- The hosts.
- The authorities.
- What a connection signed by some other authority does.

## Check

Present a certificate from an authority outside the set. The sensitive call fails. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Network security configuration](https://developer.android.com/privacy-and-security/security-config). The page supports this rule: You can limit the set of trusted CAs instead of trusting every pre-installed CA. Apps targeting older platform versions also trust the user-added CA store by default unless you customize that.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Debug trust settings do not ship](125-debug-certificates-do-not-ship.md)
