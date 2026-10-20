---
title: Web content is another trust boundary
tags: [practices, security, screen, mobile]
status: tested
updated: 2026-10-19
---

# Web content is another trust boundary

A view that renders remote pages can run script. That is a different trust boundary from the rest of the app.

## Rule

Load only the content the screen needs. Do not give remote pages a bridge into app capabilities unless every input on that page is trusted and the bridge is required.

## Specify

- Which pages the view may open.
- Whether script is enabled, and why.
- Which app methods, if any, the page can call.

## Check

Open an untrusted page in the view and confirm it cannot call an app method that reads private data. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Use addJavaScriptInterface() with particular care. If untrusted input is allowed, untrusted JavaScript might be able to invoke Android methods within your app.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A script bridge is only for trusted pages](62-script-bridge-only-for-trusted-pages.md)
