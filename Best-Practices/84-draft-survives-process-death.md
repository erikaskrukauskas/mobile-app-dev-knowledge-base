---
title: A draft survives process death
tags: [practices, state, lifecycle, offline, mobile]
status: tested
updated: 2026-10-19
---

# A draft survives process death

A draft is user work. Process death is normal while they are in another app.

## Rule

Persist the draft before the process can die. Restoring the screen shows the draft. Dismissing the draft is a separate, explicit action.

## Specify

- When the draft is written.
- What restore shows.
- How the person discards it.

## Check

Type a draft, stop the process, and reopen. The draft is back. Discard it and it stays gone. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: Use local persistence to handle process death for complex or large data. A draft is that data.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Keep process-death state small](16-small-saved-state.md)
- [User work is not cache](28-user-work-is-not-cache.md)
