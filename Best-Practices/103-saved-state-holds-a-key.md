---
title: Process-death memory holds a key, not the record
tags: [practices, lifecycle, state, mobile]
status: tested
updated: 2026-10-19
---

# Process-death memory holds a key, not the record

The small save that survives process death is slow to write and limited in size.

## Rule

Put an id or another small key there. Load the record from local storage. Do not put bitmaps or large structures in that save.

## Specify

- The key.
- The store that holds the record.
- The screen when the record is missing.

## Check

Restore after process death. The record loads from storage via the key. A bitmap is not required to be inside the small save. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: Use saved state to store a minimal amount of data necessary, such as an ID, to recreate the data necessary to restore the UI.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Keep process-death state small](16-small-saved-state.md)
