---
title: Losing the network mid-task is a named state
tags: [practices, offline, error, screen, mobile]
status: tested
updated: 2026-10-19
---

# Losing the network mid-task is a named state

A transfer or a call that loses the network is not the same as the person pressing stop.

## Rule

Name the interrupted state, say what was kept, and say whether it will resume on its own. Do not mark the task finished.

## Specify

- The interrupted state.
- The resume rule.
- The stop rule, which is different.

## Check

Drop the network during the task. The status and the screen show interrupted, not finished. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Read network state](https://developer.android.com/develop/connectivity/network-ops/reading-network-state). The page supports this rule: When a network disconnects, that network object stops being usable. The task has to notice the change rather than assume the work completed.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A stopped transfer says what was kept](171-partial-result-of-a-stopped-transfer-is-named.md)
- [Listen for network changes instead of polling](163-listen-for-network-changes.md)
