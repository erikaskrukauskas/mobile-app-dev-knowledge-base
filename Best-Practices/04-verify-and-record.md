---
title: Verify on a mobile client, then record
tags: [practices, testing, lessons, mobile]
status: verified
updated: 2026-10-19
---

# Verify on a mobile client, then record

Call the work done after a test or an exercised user path on a mobile client. Then record a lesson when a later mobile project would otherwise repeat the same investigation.

## The check

Name the check before implementation, in the same place as the screen behavior and the boundary. See [Specify the screen and done](02-specify-screen-and-done.md).

A fitting check is one of these:

- An automated test that runs against a mobile client, a device, or an emulator and asserts the screen or platform behavior.
- A written user path someone exercises on a phone: the start screen, the actions, and the result they can see.
- Both, when the risk is a permission, offline state, or a lifecycle transition that a unit test on the host would miss.

"It compiles" and "the preview looks right" are not the check when the promise is about navigation, lifecycle, offline behavior, a permission, or accessibility on a phone.

Confirm the current testing tool before you rely on a feature of it. Entry points are in [Official-Documentation/README.md](../Official-Documentation/README.md).

## When to record

Add a file under `Lessons-Learned/` when the finding is reusable: another mobile project could hit the same screen, lifecycle, offline, permission, or accessibility constraint.

Leave the note in the project when it depends on that product's requirements, environment names, credentials, bundle identifiers, or local architecture. See [Practice versus project](05-practice-versus-project.md).

Use [Lessons-Learned/_template.md](../Lessons-Learned/_template.md). Set status to `candidate` until the check has been reviewed, and `tested` when the check was run in this environment. Set `verified` only when another session can apply the lesson without re-discovering the dead ends.

## Where the lesson goes

- A reusable mobile lesson is written here.
- A general application lesson is written in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).
- An AI-tooling lesson is written in the [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base).

When one effort produces more than one kind of lesson, write each lesson in its repo and link the others. Do not paste the same write-up into two libraries.

## Replacement

When a newer lesson or practice replaces this one, set the old document to `superseded`, set `superseded_by` to the replacement path, and keep the file.
