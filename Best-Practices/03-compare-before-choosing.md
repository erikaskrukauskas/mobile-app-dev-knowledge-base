---
title: Compare before choosing
tags: [practices, navigation, screen, state, mobile]
status: verified
updated: 2026-10-19
---

# Compare before choosing

Name the real options before choosing navigation, a screen contract, or where mobile state lives. Then implement one. A single favorite presented as the only possibility is a skipped comparison.

## Decisions that need options

- Navigation: how a person moves between screens, how they return, and what happens to the screen they left. Write at least two arrangements that could satisfy the same journey.
- Screen contract: what a screen shows, what it accepts, and what it promises will still be true after the person leaves and comes back. Include the empty, loading, and error appearances when the screen can be in those states.
- Where mobile state lives: memory for the current screen, a local store on the device, or a remote store reached over the network. Offline behavior is part of this choice. Say what the person can still do when the network is absent, and what waits until the network returns.
- Lifecycle: what must be saved or released when the app backgrounds, and what must be refreshed when it resumes. Compare keeping work in memory with writing it to local state before the system can stop the process.

A framework, language, or platform is an implementation option, not the practice. Record it on an [official-doc pointer](../Official-Documentation/README.md) when the decision depends on a current platform feature. Confirm that page before relying on the feature.

## What to write down

For each option, state:

- The screen or platform behavior a person can observe.
- The boundary: which screen, store, or permission the option touches.
- What fails, and what the person sees.
- The check that would show this option works on a mobile client.

Then say which option you will implement and why the others were set aside. The reason should still make sense after the product's name is removed.

## Rules that stay in the other library

A choice about a public HTTP API, a shared state rule any client could use, or application security that does not depend on the device belongs in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base). Compare the mobile consequence here, and link that repo for the general rule.

## After the choice

Implement the chosen option. Run the check named in [Verify on a mobile client, then record](04-verify-and-record.md). If the comparison itself would help another mobile project, record it as a lesson after the check.
