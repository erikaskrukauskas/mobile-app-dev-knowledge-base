---
title: Debug trust settings do not ship
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# Debug trust settings do not ship

A certificate added so a developer can inspect traffic must not be trusted by the build people install.

## Rule

Keep extra debug trust in the debug configuration only. The release build trusts the named production authorities and not the debug ones.

## Specify

- What the debug build trusts.
- What the release build trusts.

## Check

Install the release build and confirm the debug authority is not trusted. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Network security configuration](https://developer.android.com/privacy-and-security/security-config). The page supports this rule: The network security configuration includes debug-only overrides so you can debug secure connections without added risk to the installed base.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A release build limits logs](94-release-build-limits-logs.md)
