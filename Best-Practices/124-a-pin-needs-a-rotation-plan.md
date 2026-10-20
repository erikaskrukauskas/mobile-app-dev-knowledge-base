---
title: A certificate pin needs a way to rotate
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# A certificate pin needs a way to rotate

A pin that only matches today's key strands every installed app when the key changes.

## Rule

If you pin, include a backup key and write down how a key change reaches people without an emergency binary update. An expiry that disables the pin is a weaker guarantee. Name that tradeoff if you use one.

## Specify

- The pins.
- The backup key.
- How a rotation ships.

## Check

Review the pin set and the rotation note. A second key is present, or the page explains why the app will ship an update before the current key ends. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Network security configuration](https://developer.android.com/privacy-and-security/security-config). The page supports this rule: When using certificate pinning, you should always include a backup key so that if you are forced to switch keys or CAs, connectivity is unaffected. Otherwise you must ship an update to restore connectivity.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Cleartext network access stays off](123-cleartext-stays-off.md)
