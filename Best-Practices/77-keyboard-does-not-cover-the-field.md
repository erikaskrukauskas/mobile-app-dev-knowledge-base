---
title: The keyboard does not cover the focused field
tags: [practices, screen, accessibility, mobile]
status: tested
updated: 2026-10-19
---

# The keyboard does not cover the focused field

A software keyboard can sit on top of the field the person is typing into, and on top of the error under it.

## Rule

When the keyboard is open, the focused field and its error text stay on screen, by scrolling if needed.

## Specify

- The fields that open a keyboard.
- What must stay visible.
- What happens on a small phone.

## Check

Focus the last field on a small phone. The field and its label stay visible with the keyboard open. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Build accessible apps](https://developer.android.com/guide/topics/ui/accessibility). The page supports this rule: An accessible flow has to be operable. A field hidden by the keyboard cannot be operated or checked.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Point an error at the field](40-name-the-field-that-failed.md)
