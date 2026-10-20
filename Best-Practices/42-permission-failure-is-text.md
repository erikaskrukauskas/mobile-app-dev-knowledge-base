---
title: A denied permission is explained in text
tags: [practices, error, permissions, accessibility, mobile]
status: tested
updated: 2026-10-19
---

# A denied permission is explained in text

A system dialog can close and leave the screen looking unchanged. The person may not know the action was refused.

## Rule

After a denial, the screen says what did not happen and what they can do next. The explanation is text, not color alone.

## Specify

- The text after denial.
- The next step, including a settings path when the platform will not ask again.
- The text after a later grant.

## Check

Deny the permission. The screen's text names the blocked action. Grant it later and the action becomes available. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: When you make a permissions request, be clear about what you're accessing, why, and what functionalities are affected if permissions are denied.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A permanent denial has a way forward](50-permanent-denial-path.md)
- [Mobile application security](06-mobile-application-security.md)
