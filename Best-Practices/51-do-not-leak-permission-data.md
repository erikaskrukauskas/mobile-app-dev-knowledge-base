---
title: Do not hand permission-only data to another app
tags: [practices, security, permissions, mobile]
status: tested
updated: 2026-10-19
---

# Do not hand permission-only data to another app

Data the app can read only because it holds a permission is still restricted.

## Rule

Do not pass that data to another app, a log, or a web view that does not itself hold the same access. Share a narrower export if the person asked to share one item.

## Specify

- Which data is permission-only.
- Which paths can leak it.
- The share path that sends one chosen item.

## Check

Attempt to share a permission-only collection with another app. Only the item the person chose leaves, or nothing does. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Don't leak permission-protected data. This occurs when your app exposes data over IPC that is available only because your app has permission to access that data.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Share only what the screen allows](88-share-out-only-what-the-screen-allows.md)
