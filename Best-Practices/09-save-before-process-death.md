---
title: Save state before process death
tags: [practices, lifecycle, state, offline, mobile]
status: tested
updated: 2026-10-19
---

# Save state before process death

The person expects a screen to look the same when they switch away and come back. The system may destroy the process while they are gone.

## Rule

Save the smallest state needed to rebuild the screen before the process can die. Memory that lives only inside the running process is not that save.

## Specify

- What must reappear: the draft, the scroll place, the selected item, or the step in a flow.
- Where that state is written before the process stops.
- What a cold start shows if the save is missing.

## Check

Background the app, stop the process, and reopen the same screen. The named state is still there. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: Users expect the UI state to stay the same, but the system might destroy the activity hosting the screen and its stored state.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Keep input across a configuration change](11-keep-state-across-configuration-change.md)
- [Keep process-death state small](16-small-saved-state.md)
