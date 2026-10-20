---
title: A playback notice is not a promotional alert
tags: [practices, screen, permissions, mobile]
status: tested
updated: 2026-10-19
---

# A playback notice is not a promotional alert

The notice that says audio is playing is part of that task. A marketing alert is a different decision.

## Rule

Keep the ongoing playback or call notice tied to that task. Do not use an exemption for that notice as permission to send other alerts after the person has refused alerts.

## Specify

- Which notices are part of an ongoing task.
- Which alerts stop when they refuse notifications.

## Check

Refuse alerts, start playback, and confirm the playback notice matches the task. Confirm a promotional alert is not posted. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: Notifications related to media sessions can be exempt from the notification-permission change. A denial still blocks ordinary notification channels.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Ongoing work the person is not watching is still visible](109-ongoing-work-is-visible.md)
- [Check that alerts are allowed before you send one](118-check-before-you-notify.md)
