---
title: The permission prompt matches a decision the person can understand
tags: [practices, permissions, screen, mobile]
status: tested
updated: 2026-10-19
---

# The permission prompt matches a decision the person can understand

A prompt that does not say what is being allowed is not a decision.

## Rule

The moment before the prompt, the screen says what the app will access and what fails if they refuse. Confirm the platform's required reason text before shipping a prompt.

## Specify

- The reason on the screen.
- The platform reason text, confirmed against current docs.
- The result of allow and of refuse.

## Check

Trigger the prompt. The reason is visible before the system dialog. Refuse and allow both match the copy. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: Be transparent. When you make a permissions request, be clear about what you're accessing, why, and what functionalities are affected if permissions are denied.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A denied permission is explained in text](42-permission-failure-is-text.md)
- [Mobile application security](06-mobile-application-security.md)
