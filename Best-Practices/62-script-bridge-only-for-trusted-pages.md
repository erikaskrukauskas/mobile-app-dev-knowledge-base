---
title: A script bridge is only for trusted pages
tags: [practices, security, mobile]
status: tested
updated: 2026-10-19
---

# A script bridge is only for trusted pages

A bridge lets page script call into the app. That is app-level power.

## Rule

Expose a bridge only to pages shipped with the app, or to pages whose input you fully trust. Leave it off for ordinary web content. Leave script itself off when the screen does not need it.

## Specify

- Whether script is on.
- Whether a bridge exists.
- The pages that may use it.

## Check

Load an untrusted URL and confirm the bridge methods are unreachable. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: In general, we recommend exposing addJavaScriptInterface() only to JavaScript that is contained within your application APK. If your application doesn't directly use JavaScript within a WebView, don't call setJavaScriptEnabled.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Web content is another trust boundary](53-web-content-is-another-trust-boundary.md)
