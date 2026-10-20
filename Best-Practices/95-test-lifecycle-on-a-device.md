---
title: Test lifecycle on a device or emulator
tags: [practices, testing, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Test lifecycle on a device or emulator

A host unit test does not rotate the device or kill the process.

## Rule

Run the lifecycle checks on a device or an emulator: background, process death, and return. Name that check in the specification.

## Specify

- The device or emulator.
- The steps.
- The state that must survive.

## Check

Run the named steps. The screen matches [Save state before process death](09-save-before-process-death.md) and [Resume the same task](13-resume-the-same-task.md). Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Test apps on Android](https://developer.android.com/training/testing). The page supports this rule: Instrumented tests run on devices or emulators so you can verify behavior that a host unit test does not host.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Verify on a mobile client, then record](04-verify-and-record.md)
- [Save state before process death](09-save-before-process-death.md)
