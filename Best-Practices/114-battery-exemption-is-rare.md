---
title: A battery exemption is a rare, named exception
tags: [practices, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# A battery exemption is a rare, named exception

Asking the person to ignore battery limits so the app can sync is not a default setup step.

## Rule

Do not ask them to exempt the app unless idle limits break the core function and a normal push cannot do the job. If you ask, the screen says what breaks without the exemption.

## Specify

- The core function that breaks.
- Why a normal push is not enough.
- The path that does not ask, for every other function.

## Check

Install the app and use the main path. No exemption prompt appears. The rare function, if you have one, explains the ask. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Most apps can send the person to battery settings. Asking directly to be exempted is for an acceptable use case, and store policy can forbid the direct ask unless the core function is adversely affected.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Do not stay awake just to avoid being treated as idle](111-do-not-stay-awake-to-look-busy.md)
