---
title: Test with the platform assistive technology
tags: [practices, testing, accessibility, mobile]
status: tested
updated: 2026-10-19
---

# Test with the platform assistive technology

An automated contrast check does not prove a screen reader can finish the task.

## Rule

Run the main path with the platform screen reader on a device. Record the path and the result. Automated checks can sit beside that path. They do not replace it.

## Specify

- The screen reader.
- The path.
- The announcements that must occur.

## Check

Complete the path with the screen reader. The result matches [The whole flow works with assistive technology](73-flows-work-with-assistive-tech.md). Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Build accessible apps](https://developer.android.com/guide/topics/ui/accessibility). The page supports this rule: The Android accessibility guide tells you to test with tools such as the Accessibility Scanner and with checks of the user flows.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The whole flow works with assistive technology](73-flows-work-with-assistive-tech.md)
