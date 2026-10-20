---
title: A pin failure has a screen, not a crash
tags: [practices, security, error, mobile]
status: tested
updated: 2026-10-19
---

# A pin failure has a screen, not a crash

A pin that no longer matches is a connectivity failure. The person cannot fix a certificate.

## Rule

Show the same class of message as a failed protected connection, keep local data, and do not fall back to cleartext. The rotation plan is how you prevent this, not a runtime prompt that asks them to ignore the error.

## Specify

- The message.
- That cleartext is not the fallback.
- That local data remains.

## Check

Fail the pin in a test build. The screen shows the connection failure and does not offer to proceed anyway. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Network security configuration](https://developer.android.com/privacy-and-security/security-config). The page supports this rule: Pinning fails closed when the key does not match. The documented escape is a backup key or an app update, not an on-the-spot bypass.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A certificate pin needs a way to rotate](124-a-pin-needs-a-rotation-plan.md)
- [Cleartext network access stays off](123-cleartext-stays-off.md)
