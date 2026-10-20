---
title: Ongoing work usually starts from a tap
tags: [practices, lifecycle, screen, mobile]
status: tested
updated: 2026-10-19
---

# Ongoing work usually starts from a tap

The usual reason ongoing work is allowed is that the person just asked for it.

## Rule

Start playback, recording, or a watched transfer from the control they used. Do not start that class of work from a silent push.

## Specify

- The controls that start it.
- The pushes that do not.

## Check

Send a silent push. Ongoing work does not start. Tap the control. It starts, with a visible status. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: Examples of foreground work are playback and a fitness session the person started. Starting that work from the background is restricted.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Ongoing work names why it is allowed to continue](143-ongoing-work-names-its-reason.md)
- [Do not promote a background job into ongoing work](144-do-not-promote-idle-work-to-ongoing.md)
