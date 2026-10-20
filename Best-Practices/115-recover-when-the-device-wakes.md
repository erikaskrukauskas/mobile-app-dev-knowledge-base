---
title: The app recovers when the device leaves idle
tags: [practices, lifecycle, error, mobile]
status: tested
updated: 2026-10-19
---

# The app recovers when the device leaves idle

After a long idle period, the next open should look like a normal open, not a crash or a wiped draft.

## Rule

When the device wakes or the person opens the app, resume from saved state, run waiting work that is still relevant, and drop work that expired. Do not show a stack of failures for jobs the system deferred on purpose.

## Specify

- What resumes.
- What is discarded because it expired.
- What the first screen shows.

## Check

Force the device through an idle period, wake it, and open the app. Drafts remain and the screen is usable. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: When the user wakes the device by moving it, turning on the screen, or connecting a charger, the system exits Doze and all apps resume normal activity. Test that the app recovers gracefully.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Resume the same task](13-resume-the-same-task.md)
- [Background sync may wait until the device is idle-awake](112-background-sync-may-wait.md)
