---
title: Clear a web view that showed sensitive content
tags: [practices, security, state, mobile]
status: tested
updated: 2026-10-19
---

# Clear a web view that showed sensitive content

A web view can keep files for pages it showed, including pages that contained private data.

## Rule

When the person signs out, or when the screen was showing sensitive content, clear that local web cache. Prefer responses that say they must not be stored when you control the server.

## Specify

- When the cache is cleared.
- What the next person can still open inside the view.

## Check

Open a sensitive page, sign out, and reopen the view. The sensitive page is not available from the cache. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: If your application accesses sensitive data with a WebView, consider using the clearCache() method to delete any files stored locally.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Web content is another trust boundary](53-web-content-is-another-trust-boundary.md)
- [Sign-out clears private local data](30-sign-out-clears-private-data.md)
