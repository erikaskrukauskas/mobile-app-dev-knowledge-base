---
title: A reboot does not throw away local work
tags: [practices, state, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# A reboot does not throw away local work

Unlocking after a reboot is not a new account and not a reason to drop drafts that were in the private store.

## Rule

After unlock, private drafts and records are still there. Only data you deliberately keep out of that store is gone. Say so if a before-unlock task could not run.

## Specify

- What survives reboot.
- What does not.
- The message if a before-unlock task was skipped.

## Check

Create a draft, reboot, unlock. The draft is there. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: Credential encrypted storage remains the store for private data across a restart, and it becomes available again when the user unlocks the device.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A draft survives process death](84-draft-survives-process-death.md)
- [The default store is the one that needs unlock](155-the-default-store-needs-unlock.md)
