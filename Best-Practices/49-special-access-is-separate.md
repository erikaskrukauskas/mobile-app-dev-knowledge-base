---
title: Access while the app is hidden is a separate decision
tags: [practices, permissions, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Access while the app is hidden is a separate decision

Using the camera, microphone, or location while the person is looking at the screen is not the same decision as using them while the app is hidden.

## Rule

Treat background or special access as its own permission decision, with its own reason and its own denial path. Do not reuse the foreground grant as if it covered the hidden case.

## Specify

- What runs only while the screen is visible.
- What is proposed while the app is hidden.
- The separate prompt or settings step.

## Check

Grant only the foreground permission and background the app. The hidden capability does not run. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: Special permissions correspond to particular app operations. The platform defines them when it wants to protect access to particularly powerful actions.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Release work when the app is not visible](12-release-work-when-backgrounded.md)
- [Recheck a permission before each use](45-recheck-before-each-use.md)
