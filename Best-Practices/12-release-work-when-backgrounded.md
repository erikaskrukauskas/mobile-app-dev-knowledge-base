---
title: Release work when the app is not visible
tags: [practices, lifecycle, state, mobile]
status: tested
updated: 2026-10-19
---

# Release work when the app is not visible

A screen that keeps a camera, a location stream, or a playback session running after the person has left spends the device and can surprise them.

## Rule

Stop work that only makes sense while the screen is visible. Resume it from the same spot when they return, if the task is still theirs.

## Specify

- What stops when the screen is no longer visible.
- What is allowed to continue, and why the person can tell.
- What resumes, and from which point.

## Check

Start the work, switch to another app, and confirm the work has stopped. Return and confirm it continues from the named point. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [The activity lifecycle](https://developer.android.com/guide/components/activities/activity-lifecycle). The page supports this rule: If you're building a streaming video player, you might pause the video and terminate the network connection when the user switches to another app. When the user returns, you can reconnect to the network and let the user resume the video from the same spot.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Resume the same task](13-resume-the-same-task.md)
