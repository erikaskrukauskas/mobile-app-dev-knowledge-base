---
title: Test standby separately from device idle
tags: [practices, testing, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Test standby separately from device idle

The whole device being asleep and this app being unused are different restrictions.

## Rule

Run both checks. Device idle covers the dark unplugged phone. App standby covers this app being unused while the phone is otherwise awake. Both should recover cleanly.

## Specify

- The device-idle steps.
- The app-standby steps.
- The expected screen after each.

## Check

Run both. Saved work remains and there is no decoy notification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: The Doze test and the App Standby test are separate procedures. After waking the app from standby, notifications and jobs should behave as you specified.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Test the app on an idle device](148-test-the-idle-device.md)
