---
title: A call-style notice is only for a call
tags: [practices, screen, permissions, mobile]
status: tested
updated: 2026-10-19
---

# A call-style notice is only for a call

Platforms exempt some call-style notices from the ordinary alert permission. That exemption is not a costume for other messages.

## Rule

Use a call-style ongoing notice only for an actual call the person is handling. Every other alert follows the ordinary permission.

## Specify

- What counts as a call.
- What does not.

## Check

Trigger a non-call event with alerts denied. No call-style notice appears. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: Apps configured to self-manage phone calls can send call-style notices without the ordinary notification permission. That path is for those call notices.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A playback notice is not a promotional alert](121-playback-notice-is-not-a-promotion.md)
