---
title: A network failure says what still works
tags: [practices, error, offline, screen, mobile]
status: tested
updated: 2026-10-19
---

# A network failure says what still works

A failed request is not the same as an empty screen, and it is not the same as a loss of local data.

## Rule

Say that the network step failed, whether stored data is on screen, and what the person can retry. Leave local user work in place.

## Specify

- The message.
- What remains usable.
- What retry does.

## Check

Disable the network in the middle of a refresh. The screen names the failure and keeps the local work. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [The activity lifecycle](https://developer.android.com/guide/components/activities/activity-lifecycle). The page supports this rule: The lifecycle guidance treats a lost network as something the app can resume from, rather than as a wiped task.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Show the age of offline data](27-show-data-age-when-offline.md)
- [An offline command applies once](29-offline-command-applies-once.md)
