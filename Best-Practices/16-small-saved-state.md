---
title: Keep process-death state small
tags: [practices, lifecycle, state, mobile]
status: tested
updated: 2026-10-19
---

# Keep process-death state small

The bundle that survives process death is for a small key, not for the whole record.

## Rule

Store an identifier or another small value in the process-death save. Put large or complex data in local storage, and load it from that id after restore.

## Specify

- The small key that is saved.
- The store that holds the large data.
- The behavior when the large data is gone.

## Check

Restore after process death with a large draft. The draft comes back from local storage, and the restore does not depend on stuffing the draft into the small save. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: Don't use saved state to store large amounts of data, such as bitmaps, nor complex data structures that require lengthy serialization or deserialization.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Save state before process death](09-save-before-process-death.md)
- [User work is not cache](28-user-work-is-not-cache.md)
