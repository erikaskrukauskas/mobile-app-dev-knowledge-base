---
title: Private files stay in app storage
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Private files stay in app storage

Files that only this app should read belong in storage the platform keeps private to the app.

## Rule

Write private files to app-private storage. Do not mark them world-readable so another app can open them.

## Specify

- Which files are private.
- The store they use.
- How another app is given a file when sharing is intentional.

## Check

After saving a private file, confirm another app on the device cannot read it. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: By default, files that you create on internal storage are accessible only to your app.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [External storage is untrusted](31-external-storage-is-untrusted.md)
- [Sharing stored data with other apps is explicit](36-exported-store-is-explicit.md)
