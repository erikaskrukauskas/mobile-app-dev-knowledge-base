---
title: An accessibility helper that runs before unlock stays limited
tags: [practices, accessibility, security, mobile]
status: tested
updated: 2026-10-19
---

# An accessibility helper that runs before unlock stays limited

An accessibility service is one of the few reasons to run before unlock. That does not entitle it to the mailbox.

## Rule

A before-unlock accessibility helper does its assistive job without reading private records. Private content is announced only after unlock.

## Specify

- What it may do before unlock.
- What it reads only after unlock.

## Check

Reboot, stay locked, and use the helper. Private records are not spoken. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Support Direct Boot mode](https://developer.android.com/training/articles/direct-boot). The page supports this rule: Accessibility services such as a screen reader are a documented reason to run during Direct Boot. Private user information still belongs in credential encrypted storage.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Work before unlock is a small, explicit component](117-before-unlock-work-is-explicit.md)
