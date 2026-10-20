---
title: Do not fight the idle bucket
tags: [practices, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Do not fight the idle bucket

Trying to stay in the most active bucket is the same mistake as asking for a battery exemption.

## Rule

Accept that an unused app will be restricted. Make the next open correct. Do not add fake notifications or fake foreground work to stay active.

## Specify

- The next-open behavior.
- The tricks you will not use.

## Check

Leave the app unused. It does not post decoy notifications. Opening it later shows saved work. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Standby is based on the person not using the app. A visible notification or a foreground service is a real task, not a way to stay out of standby.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Standby means they have not been using the app](169-standby-means-they-have-not-used-the-app.md)
