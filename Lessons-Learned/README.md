---
title: Lessons learned
tags: [lessons, index, testing]
status: verified
updated: 2026-10-19
---

# Lessons learned

Lessons are evidence from real mobile work. Best-practice pages are the stable rules. A lesson becomes a practice only after the reusable part still holds with the original project's constraints removed.

## Lifecycle

`candidate` → `tested` → `verified`

| Status | Set it when |
| --- | --- |
| `candidate` | The finding is written down and has not been re-checked |
| `tested` | The check was reproduced on a mobile client, or the evidence was reviewed in this environment |
| `verified` | Another session can apply the mobile lesson without re-discovering the dead ends |
| `superseded` | A newer lesson or practice page replaces it |

Superseded files stay in the folder. Set `superseded_by` to the replacement path. Do not delete them.

## File names

`LL-0001-short-slug.md`

Increment the number. Do not reuse an id.

## What to record

Use [_template.md](_template.md). A useful lesson includes the environment, the approaches that failed, the working approach, and the check that showed it worked on a mobile client.

Record a mobile lesson here: app structure, navigation, a screen contract, lifecycle, offline and local state, platform permissions, mobile accessibility, mobile error handling, or mobile application security. Record a general application lesson in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base). Record an AI-tooling lesson in the [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base). If more than one exists, link them.

## Current lessons

| ID | Title | Status |
| --- | --- | --- |
| [LL-0001](LL-0001-mobile-application-development-only.md) | Keep this repo to mobile application development | verified |
