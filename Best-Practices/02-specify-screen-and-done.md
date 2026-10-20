---
title: Specify the screen and done
tags: [practices, screen, testing, mobile]
status: verified
updated: 2026-10-19
---

# Specify the screen and done

Describe the mobile change as screen or platform behavior, a boundary, and the check that defines done. A topic name is not a specification.

## Include

- The behavior a person can observe on the device: what they do, what the screen shows, and what stays unchanged. Include lifecycle moments that change that behavior, such as start, background, and resume, when the change depends on them.
- The boundary: which screen, navigation path, permission, or local store is in scope, and which neighboring system is out of scope. A public HTTP API that any client could call is out of scope here; link the application-development knowledge base for that contract.
- The failure behavior: what the person sees when input is rejected, the network is absent, a permission is denied, or a local store fails. That is the mobile error handling for this change.
- The check that defines done: a test on a mobile client, an exercised user path on a phone or emulator, or both. Name the command or the steps.
- Constraints that are easy to violate: a screen contract, data kept on the device, an accessibility requirement, a permission prompt, or a file the change must leave alone.

## Leave out

- A tour of unrelated product history.
- A framework, language, or platform presented as the requirement. The requirement is the behavior. The toolkit is an implementation option. See [Compare before choosing](03-compare-before-choosing.md).
- Copies of entire platform manuals. Link the canonical page in [Official-Documentation/README.md](../Official-Documentation/README.md).

## Size the change

Ask for one observable outcome when later steps depend on it. A request that mixes a new navigation model, a new offline store, and a visual redesign is harder to check on a device and easier to leave half done.

## Revision

When the result misses the mark, add the missing screen behavior or boundary to the specification. Say which check failed. A restatement that does not name the miss produces another broad attempt.

## For pages in this repo

A documentation change names the decision, the audience (a later mobile project), and the page to update. New pages are for new topics. Existing topics are edited in place. See [Write findable pages](08-write-findable-pages.md).
