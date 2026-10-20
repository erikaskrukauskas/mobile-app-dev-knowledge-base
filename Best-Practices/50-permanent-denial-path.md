---
title: A permanent denial has a way forward
tags: [practices, permissions, screen, error, mobile]
status: tested
updated: 2026-10-19
---

# A permanent denial has a way forward

After a person denies a prompt enough times, the platform may stop showing it.

## Rule

The screen still explains the block and offers the path the platform provides to settings, when one exists. Confirm that path against the current platform page. Do not loop a prompt the system will not show.

## Specify

- How the screen detects that the prompt will not appear.
- The settings path.
- What the screen offers if they never grant it.

## Check

Deny until the system stops asking, then trigger the action. The screen shows the forward path and does not re-call a prompt that will not appear. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Permissions on Android](https://developer.android.com/guide/topics/permissions/overview). The page supports this rule: The permissions guide distinguishes install-time, runtime, and special permissions, and tells you not to assume a grant. A refusal that sticks needs a specified screen, not another identical prompt.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A denied permission is explained in text](42-permission-failure-is-text.md)
