---
title: Review alerts against the current grant
tags: [practices, testing, permissions, mobile]
status: tested
updated: 2026-10-19
---

# Review alerts against the current grant

An alert feature that was only tested while notifications were on misses the default-off install.

## Rule

Test a fresh install with alerts off, a denial, a dismiss of the prompt, and a restore that already has the grant. Each one matches the alert rules. The in-app state stays intact in all four.

## Specify

- The four setups.
- The expected alerts.
- The expected in-app state.

## Check

Run the four setups on a device. They match the specification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Notification runtime permission](https://developer.android.com/develop/ui/views/notifications/notification-permission). The page supports this rule: The notification-permission guide includes how a new install, a denial, a dismissed dialog, and a restore behave, and how to test those sequences.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A new install cannot notify until the person allows it](120-a-new-install-cannot-notify-yet.md)
- [A restored app may already allow alerts](164-a-restored-app-may-already-allow-alerts.md)
