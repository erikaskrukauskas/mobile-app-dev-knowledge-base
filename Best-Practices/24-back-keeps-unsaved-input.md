---
title: Back does not silently drop unsaved input
tags: [practices, navigation, screen, state, mobile]
status: tested
updated: 2026-10-19
---

# Back does not silently drop unsaved input

The system back gesture can pop a screen that still holds what the person typed.

## Rule

If leaving would discard input they have not saved, ask before leaving, or save a draft. A gesture that throws the input away with no signal is a failed check.

## Specify

- Which screens hold unsaved input.
- Whether back saves a draft or asks.
- What cancel does.

## Check

Type into a field and use the system back gesture. The input is kept, or the screen asks before discarding it. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: The user expects that when they navigate to a screen, its transient UI state remains the same until they completely dismiss it.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Back returns to the previous place](17-back-returns-to-previous.md)
- [A draft survives process death](84-draft-survives-process-death.md)
