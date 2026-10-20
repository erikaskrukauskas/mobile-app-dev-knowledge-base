---
title: A destructive action confirms on the device
tags: [practices, screen, error, mobile]
status: tested
updated: 2026-10-19
---

# A destructive action confirms on the device

Delete, send, and pay are hard to undo. A single stray tap should not complete them.

## Rule

Ask for a confirmation that names the consequence, or provide an undo that is actually available. The confirmation itself is a screen with text, not color alone.

## Specify

- Which actions confirm.
- The words of the confirmation.
- What undo covers, if you offer undo instead.

## Check

Start the action and cancel the confirmation. The record is unchanged. Confirm it in a second run and the record changes once. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 3.3.1: Error Identification](https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html). The page supports this rule: Error identification is about the person understanding what happened. A destructive confirm is the same duty before the change: the consequence is in text.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Dismissing a modal is an explicit choice](26-modal-dismiss-is-explicit.md)
