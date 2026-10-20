---
title: An empty screen says why it is empty
tags: [practices, screen, error, mobile]
status: tested
updated: 2026-10-19
---

# An empty screen says why it is empty

An empty list can mean the person has no items, the filter excluded them, or the load failed.

## Rule

The empty appearance says which case it is and what the person can do next. It does not reuse the failure message for a genuinely empty collection.

## Specify

- The empty case.
- The filtered case.
- The failure case, which is not this one.

## Check

Open the screen with no items, with a filter that matches nothing, and with a failed load. The three appearances differ. Run it on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).

## Source

Checked 2026-10-19. [Understanding Success Criterion 3.3.1: Error Identification](https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html). The page supports this rule: An error must be indicated in text. An empty collection that is not an error needs different text, or the person cannot tell them apart.

Confirm that page before you rely on a platform feature. This practice does not pick a framework, a language, or a platform. A general application rule that any client could use stays in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Related

- [A local store failure is visible](38-local-store-failure-is-visible.md)
- [A loading screen says it is waiting](80-loading-state-says-waiting.md)
