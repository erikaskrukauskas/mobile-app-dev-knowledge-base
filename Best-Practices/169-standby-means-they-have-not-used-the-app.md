---
title: Standby means they have not been using the app
tags: [practices, lifecycle, mobile]
status: tested
updated: 2026-10-19
---

# Standby means they have not been using the app

An app they have not opened, and that is not doing a task they expect, will be treated as idle.

## Rule

Design the quiet state so being idle is fine: local data remains, and the next open refreshes. Do not fight standby with a permanent notification they did not ask for.

## Specify

- What still works after days unused.
- What refreshes on next open.
- The notification you will not post.

## Check

Mark the app inactive, wait, and open it. Data they saved is there. No phantom ongoing notification was posted. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Optimize for Doze and App Standby](https://developer.android.com/training/monitoring-device-state/doze-standby). The page supports this rule: App Standby treats an app as idle when the person is not using it, it is not in the foreground, and it is not showing a notification they see. Don't post a foreground notification just to avoid that.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Do not stay awake just to avoid being treated as idle](111-do-not-stay-awake-to-look-busy.md)
