---
title: A stopped transfer says what was kept
tags: [practices, error, offline, screen, mobile]
status: tested
updated: 2026-10-19
---

# A stopped transfer says what was kept

Stopping a long upload or download can leave a partial file. The screen has to say whether that partial file is usable.

## Rule

When they stop a transfer, or the system stops it, say whether the partial result was kept, discarded, or can be resumed. Do not leave a corrupt-looking record with no explanation.

## Specify

- What stop does.
- Whether resume is possible.
- The text.

## Check

Start a large transfer and stop it halfway. The screen matches the specification. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: The person can stop a foreground task. The screen still has to say the outcome, the same way any other failed or cancelled action does.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The person can stop ongoing work](110-person-can-stop-ongoing-work.md)
- [A local store failure is visible](38-local-store-failure-is-visible.md)
