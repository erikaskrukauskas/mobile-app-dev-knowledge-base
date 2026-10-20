---
title: Test the missing deep link
tags: [practices, testing, navigation, error, mobile]
status: tested
updated: 2026-10-19
---

# Test the missing deep link

The happy link is the easy check. The missing record is the one that crashes.

## Rule

Open a valid link and a link to a missing or unauthorized record, from outside the app. Both match [A deep link has a fallback screen](19-deep-link-fallback.md).

## Specify

- The valid link.
- The missing link.
- The screens that appear.

## Check

Open both links from another app or a browser. The results match the specification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [About deep links](https://developer.android.com/training/app-links). The page supports this rule: The deep link guide exists so you can create and test links that bring people into content. A missing target is part of that test.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A deep link has a fallback screen](19-deep-link-fallback.md)
