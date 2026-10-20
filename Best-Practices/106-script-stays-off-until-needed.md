---
title: Script in a web view stays off until a screen needs it
tags: [practices, security, screen, mobile]
status: tested
updated: 2026-10-19
---

# Script in a web view stays off until a screen needs it

Script is how a page reaches for app power. The default in the platform guidance is off.

## Rule

Leave script disabled unless this screen's specification says the page must run it. When you enable it, also apply [A script bridge is only for trusted pages](62-script-bridge-only-for-trusted-pages.md).

## Specify

- Whether this screen enables script.
- Why, if it does.
- The pages it will load.

## Check

Open the screen that should not run script and confirm script does not run. Open the screen that should and confirm only its pages load. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: By default, WebView doesn't execute JavaScript. If your application doesn't directly use JavaScript within a WebView, don't call setJavaScriptEnabled.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A script bridge is only for trusted pages](62-script-bridge-only-for-trusted-pages.md)
