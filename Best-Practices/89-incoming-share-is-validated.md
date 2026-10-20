---
title: An incoming share is validated before it is stored
tags: [practices, security, error, state, mobile]
status: tested
updated: 2026-10-19
---

# An incoming share is validated before it is stored

Another app can share a file the person did not expect, of a type or size you do not handle.

## Rule

Validate type and size before storing. Show a text error when you reject it. Do not execute a shared file.

## Specify

- The types and sizes you accept.
- The error when you reject one.
- That a shared file is never run as code.

## Check

Share an accepted file and a rejected file into the app. Only the accepted file is stored. The rejected file shows the error. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Security tips](https://developer.android.com/privacy-and-security/security-tips). The page supports this rule: Perform input validation when handling data from an untrusted source. Don't store executables on external storage prior to dynamic loading.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [Validate data that arrives from outside](37-validate-data-from-outside.md)
