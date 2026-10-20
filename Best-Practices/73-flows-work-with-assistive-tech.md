---
title: The whole flow works with assistive technology
tags: [practices, accessibility, testing, screen, mobile]
status: tested
updated: 2026-10-19
---

# The whole flow works with assistive technology

A labeled button is not a flow. The person has to start, finish, and recover.

## Rule

Exercise the main path, the empty path, and the error path with the platform screen reader. Every step can be perceived, operated, and understood.

## Specify

- The paths.
- The assistive technology.
- The step that is done when the path is finished.

## Check

Complete each path with the screen reader and without looking at the screen. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Build accessible apps](https://developer.android.com/guide/topics/ui/accessibility). The page supports this rule: The Android accessibility guide says to ensure all user flows are accessible, and to test with tools and automated checks.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Test with the platform assistive technology](97-test-with-assistive-technology.md)
- [Verify on a mobile client, then record](04-verify-and-record.md)
