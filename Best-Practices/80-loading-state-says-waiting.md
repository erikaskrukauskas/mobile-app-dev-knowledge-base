---
title: A loading screen says it is waiting
tags: [practices, screen, error, mobile]
status: tested
updated: 2026-10-19
---

# A loading screen says it is waiting

A blank screen while data loads looks like a crash or an empty account.

## Rule

While the result is not ready, show that the screen is waiting. When waiting ends, show the result, the empty state, or the error. Do not leave the waiting indicator up after a failure.

## Specify

- What waiting looks like.
- What replaces it on success, empty, and failure.

## Check

Load slowly, then fail a second run. Waiting appears, then the matching end state. The indicator does not remain after the failure. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Test apps on Android](https://developer.android.com/training/testing). The page supports this rule: Android's testing guide asks you to verify functional behavior and usability, which includes the time before a result is ready.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [An empty screen says why it is empty](79-empty-state-says-why.md)
- [A network failure says what still works](41-network-failure-names-what-remains.md)
