---
title: The release check does not trust the debug proxy
tags: [practices, testing, security, mobile]
status: tested
updated: 2026-10-19
---

# The release check does not trust the debug proxy

A test that only passes because a debug certificate is installed is not a test of the build people get.

## Rule

Run the protected-connection check on a release build that does not include debug trust. The call succeeds with the real host and fails with the debug stand-in.

## Specify

- The build.
- The success case.
- The failure case.

## Check

Run both cases on the release build. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Network security configuration](https://developer.android.com/privacy-and-security/security-config). The page supports this rule: Debug-only overrides exist so debugging does not add risk to the installed base. The release configuration is the one that ships.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Debug trust settings do not ship](125-debug-certificates-do-not-ship.md)
