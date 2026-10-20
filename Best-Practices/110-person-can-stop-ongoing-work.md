---
title: The person can stop ongoing work
tags: [practices, lifecycle, screen, mobile]
status: tested
updated: 2026-10-19
---

# The person can stop ongoing work

A task that keeps running after they leave needs a way for them to end it.

## Rule

The visible status includes a way to stop the task, or stopping the app stops the task. Stopping it does not discard a saved result they already committed.

## Specify

- How they stop it.
- What remains saved.
- What the screen shows the next time they open the app.

## Check

Start the ongoing task, then stop it from the status. The task ends and committed data remains. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: The foreground-service guidance includes stopping a foreground service and handling the case when a person stops an app that has one.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Ongoing work the person is not watching is still visible](109-ongoing-work-is-visible.md)
