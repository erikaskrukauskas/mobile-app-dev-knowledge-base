---
title: The visible ongoing status carries no secrets
tags: [practices, security, screen, mobile]
status: tested
updated: 2026-10-19
---

# The visible ongoing status carries no secrets

A status-bar notice is visible on a locked phone in many cases, and it is visible to someone looking over a shoulder.

## Rule

Put the task name in the ongoing status, not the private content, the token, or the body of a confidential message. The private content waits inside the app after unlock.

## Specify

- What the status says.
- What it never says.

## Check

Start a task that involves private data and read the status. The private content is absent. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: The notification exists to make the person aware that a task is consuming resources. It is a status, and private records belong in credential-protected storage rather than on that status.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Private data waits until the device is unlocked](116-private-data-waits-for-unlock.md)
