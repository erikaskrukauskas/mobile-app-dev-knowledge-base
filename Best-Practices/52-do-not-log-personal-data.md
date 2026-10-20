---
title: Do not log personal data on the device
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# Do not log personal data on the device

Device logs can be read by other software and often survive longer than the screen that wrote them.

## Rule

Keep personal data, tokens, and credentials out of logs. Limit logging in the build a person installs.

## Specify

- What must never be logged.
- How release logging is limited.
- A sample log line from a failing request, which has no secret.

## Check

Reproduce a failure in a release build and read the logs. The secret and the personal data are absent. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Be careful when writing to on-device logs. Inappropriate logging of user information could inadvertently leak user data to other applications.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A release build limits logs](94-release-build-limits-logs.md)
