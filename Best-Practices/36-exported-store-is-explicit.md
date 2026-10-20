---
title: Sharing stored data with other apps is explicit
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Sharing stored data with other apps is explicit

A store that other apps can read is a published surface. The default is that they cannot.

## Rule

Export a store only when another app must read or write it. Limit that access to the operation required. An unexported store stays inside the app.

## Specify

- Which store, if any, is exported.
- Who may read it and who may write it.
- What an unexpected caller receives.

## Check

From a second app, read the unexported store and fail. Read the exported store only with the allowed operation. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: If you don't intend to provide other applications with access to your ContentProvider, mark it as not exported.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Private files stay in app storage](32-private-files-stay-in-app-storage.md)
- [Do not hand permission-only data to another app](51-do-not-leak-permission-data.md)
