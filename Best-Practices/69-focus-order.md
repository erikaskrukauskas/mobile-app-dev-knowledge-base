---
title: Focus order follows the task
tags: [practices, accessibility, screen, mobile]
status: tested
updated: 2026-10-19
---

# Focus order follows the task

A screen reader and a keyboard move focus in an order. A random order hides the task.

## Rule

Focus moves in the order a person needs to understand and complete the screen: the title, the content, the actions. It does not jump to a hidden control first.

## Specify

- The focus order.
- What is skipped because it is hidden.
- Where focus lands after a dialog closes.

## Check

Complete the screen using only the screen reader or an external keyboard. The order matches the specification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Build accessible apps](https://developer.android.com/guide/topics/ui/accessibility). The page supports this rule: The Android accessibility guide says to ensure all user flows are accessible, which includes reaching each control in an order the person can follow.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The accessible name matches the visible label](70-label-matches-visible-text.md)
