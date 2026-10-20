---
title: A local store failure is visible
tags: [practices, error, state, offline, mobile]
status: tested
updated: 2026-10-19
---

# A local store failure is visible

A full disk, a locked store, or a migration failure can leave a screen with nothing to show.

## Rule

When the local store cannot be read or written, the screen says that, and what the person can do. It does not show an empty collection as if they had no data.

## Specify

- The failures the screen handles.
- The message.
- Whether a retry is safe.

## Check

Make the store unreadable and open the screen. The message names the failure. It does not look like an empty account. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 3.3.1: Error Identification](https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html). The page supports this rule: If an input error is automatically detected, the item that is in error is identified and the error is described to the user in text. A failed store is the same duty: the person can tell what went wrong.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [An empty screen says why it is empty](79-empty-state-says-why.md)
- [Name an input error in text](39-name-the-input-error-in-text.md)
