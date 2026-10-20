---
title: Do not promote a background job into ongoing work
tags: [practices, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Do not promote a background job into ongoing work

A sync that was fine to defer should not be relabeled as a user-visible task so it can start while the app is in the background.

## Rule

Ongoing visible work starts because the person started the task, or because they are already in the app. A job the system deferred stays deferred.

## Specify

- What may start while backgrounded.
- What may not.

## Check

While the app is backgrounded, confirm a deferred sync does not appear as a new ongoing status. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: There are restrictions on starting a foreground service from the background. The Doze guidance also says not to start one merely to avoid being idle.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Do not start a new flow in the background](14-no-new-flow-from-background.md)
- [Do not stay awake just to avoid being treated as idle](111-do-not-stay-awake-to-look-busy.md)
