---
title: The stop control on the status really stops the work
tags: [practices, screen, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# The stop control on the status really stops the work

A stop action that only dismisses the notice and leaves the microphone on is a lie.

## Rule

The stop control ends the work, releases the sensor or the socket, and clears the status. It does not only hide the notice.

## Specify

- The control.
- What it releases.
- The resulting screen.

## Check

Press stop on the status while recording or playing. The sensor or playback ends and the status clears. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Foreground services overview](https://developer.android.com/develop/background-work/services/foreground-services). The page supports this rule: Stopping the foreground service is a defined part of the model. The notification is how the person sees and controls that task.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [The person can stop ongoing work](110-person-can-stop-ongoing-work.md)
- [A finished task clears its status](175-a-finished-task-clears-its-status.md)
