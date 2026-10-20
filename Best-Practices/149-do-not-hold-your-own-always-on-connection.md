---
title: Do not hold a private always-on connection
tags: [practices, lifecycle, security, mobile]
status: tested
updated: 2026-10-19
---

# Do not hold a private always-on connection

One socket per app, kept open forever, is a battery cost. It also dies under idle restrictions.

## Rule

Receive remote messages through a shared push channel when the platform provides one. Do not keep a private socket open only to hear that something changed.

## Specify

- How messages arrive.
- What happens if that channel is unavailable: the screen still works from local data.

## Check

Leave the app idle and confirm it is not holding its own long-lived socket. A test message still reaches the alert path you specified. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: If your app requires downstream messaging, use a shared push channel such as FCM rather than maintaining your own persistent network connection.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Do not share secrets over a local network socket](60-do-not-use-a-local-socket-for-secrets.md)
