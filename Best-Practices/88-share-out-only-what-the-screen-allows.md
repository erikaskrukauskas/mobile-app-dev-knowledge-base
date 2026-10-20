---
title: Share only what the screen allows
tags: [practices, security, screen, mobile]
status: tested
updated: 2026-10-19
---

# Share only what the screen allows

The system share sheet sends data to another app. The person may not see every field that goes with it.

## Rule

Share the fields the screen named, and no others. Do not attach tokens, other records, or permission-only data the person did not choose.

## Specify

- What the share includes.
- What it excludes.
- What the other app can do with it.

## Check

Share an item and inspect the payload. Only the named fields are present. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Don't leak permission-protected data, and don't expose personal information you cannot justify.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Do not hand permission-only data to another app](51-do-not-leak-permission-data.md)
