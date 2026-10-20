---
title: A failed restore opens a safe screen
tags: [practices, lifecycle, navigation, error, mobile]
status: tested
updated: 2026-10-19
---

# A failed restore opens a safe screen

Saved state can be missing, too old, or from a screen that no longer exists.

## Rule

When restore fails, open a defined screen and say what could not be restored. Do not crash, and do not invent a half-built stack.

## Specify

- The safe screen.
- What the person is told.
- Which local records are left untouched.

## Check

Corrupt or delete the saved state, then reopen the app. The safe screen appears and the app stays usable. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Save UI states](https://developer.android.com/topic/libraries/architecture/saving-states). The page supports this rule: Use saved state to store a minimal amount of data necessary, such as an ID, to recreate the data necessary to restore the UI.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Save state before process death](09-save-before-process-death.md)
- [A deep link has a fallback screen](19-deep-link-fallback.md)
