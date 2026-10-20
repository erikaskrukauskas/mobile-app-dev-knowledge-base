---
title: A release build limits logs
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# A release build limits logs

A debug log that is useful on a desk is a leak on a person's phone.

## Rule

The build you ship does not emit verbose logs of requests, bodies, or personal data. A debug build may. The switch is explicit.

## Specify

- What a release log may contain.
- What it must not.
- How the debug build differs.

## Check

Reproduce a failure in the release build and read the log. Bodies and personal data are absent. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: In addition to not logging PII, limit log usage in production apps. Use debug flags and configurable logging levels.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Do not log personal data on the device](52-do-not-log-personal-data.md)
