---
title: Say when up and back differ
tags: [practices, navigation, screen, mobile]
status: tested
updated: 2026-10-19
---

# Say when up and back differ

Back follows the path the person took. Up goes to the parent in the structure. They are the same only when the path and the parent match.

## Rule

If a link opens a detail directly, say where up goes and where back goes. Do not send both to a surprising screen.

## Specify

- The parent of each detail.
- Where back goes when the detail was opened from outside.
- Where up goes in that same case.

## Check

Open a detail from a link and use both up and back. Each lands on the screen the specification named. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Navigation](https://developer.android.com/guide/navigation). The page supports this rule: The navigation component describes handling back and up actions as part of moving among destinations.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Back returns to the previous place](17-back-returns-to-previous.md)
- [A deep link has a fallback screen](19-deep-link-fallback.md)
