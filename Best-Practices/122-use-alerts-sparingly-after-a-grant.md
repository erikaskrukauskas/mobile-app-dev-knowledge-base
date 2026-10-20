---
title: A grant to alert is not a grant to alert often
tags: [practices, screen, permissions, mobile]
status: tested
updated: 2026-10-19
---

# A grant to alert is not a grant to alert often

People can see how many alerts an app sends, and they can revoke the grant.

## Rule

After they allow alerts, send the ones the feature promised. Do not add extra alerts because the grant exists. Each alert opens the screen that holds the state.

## Specify

- The events that alert.
- The events that only update the in-app screen.
- How they turn alerts off.

## Check

Allow alerts and use the app through a busy day of in-app changes. Only the promised events alert. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: After you receive approval to send notifications, use the permission responsibly. Users can see the number of daily notifications that your app sends, and they can revoke the permission at any time.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A notification opens the screen that holds the state](85-notification-opens-the-state.md)
