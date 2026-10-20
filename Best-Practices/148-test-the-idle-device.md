---
title: Test the app on an idle device
tags: [practices, testing, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Test the app on an idle device

A test on a plugged-in, awake phone never sees deferred jobs.

## Rule

Run an idle-mode check: force the device idle, leave it, wake it, and open the app. Drafts remain, deferred work does not appear as a user-facing failure, and an alert that should fire still fires.

## Specify

- The device.
- The idle steps.
- The expected screen after wake.

## Check

Run the steps. The results match the idle and recovery rules. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Test your app in Doze and App Standby. After you exit idle, make sure the app recovers gracefully.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The app recovers when the device leaves idle](115-recover-when-the-device-wakes.md)
- [Verify on a mobile client, then record](04-verify-and-record.md)
