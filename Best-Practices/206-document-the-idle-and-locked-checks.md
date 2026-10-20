---
title: The idle check and the locked check are part of done
tags: [practices, testing, lifecycle, security, mobile]
status: tested
updated: 2026-10-19
---

# The idle check and the locked check are part of done

A feature that syncs, alerts, or stores private data is not done when it works on an awake, unlocked developer phone.

## Rule

The specification names the idle check and the locked-reboot check whenever the feature syncs in the background, alerts, or stores private data. Those checks sit beside the on-screen check.

## Specify

- When the idle check applies.
- When the locked check applies.
- The expected results.

## Check

Run the checks named on the feature. Record the result. Do not mark the feature verified without them. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Test Doze, App Standby, and Direct Boot rather than assuming an awake unlocked device represents the phone your feature will live on.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Verify on a mobile client, then record](04-verify-and-record.md)
- [Test the app on an idle device](148-test-the-idle-device.md)
- [Test a reboot that stays locked](153-test-the-locked-reboot.md)
