---
title: A battery exemption lives in their settings
tags: [practices, lifecycle, screen, mobile]
status: tested
updated: 2026-10-19
---

# A battery exemption lives in their settings

The list of apps allowed to ignore battery limits is the person's list.

## Rule

Do not mark the app exempt yourself. If the core function truly qualifies, send them to the system setting and accept a refusal. The app still opens and still keeps local data if they refuse.

## Specify

- The function that qualifies.
- The settings path.
- The path when they refuse.

## Check

Refuse the exemption. The main task still opens. Local data remains. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: Users can configure exemptions in battery settings. An app can check whether it is exempt. It should not behave as if it had granted that exemption to itself.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A battery exemption is a rare, named exception](114-battery-exemption-is-rare.md)
