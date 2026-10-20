---
title: Practice versus project
tags: [practices, scope, mobile, governance]
status: verified
updated: 2026-10-19
---

# Practice versus project

Keep a reusable mobile practice in this repo. Keep a decision that only makes sense inside one product in that project.

## Belongs here

A note belongs here when a future mobile project, with this product's name removed, could still apply it:

- How screens are structured and how navigation returns the person to a known place.
- What a screen contract must state: contents, actions, and the empty, loading, and error appearances.
- How lifecycle, offline behavior, and local state are specified and checked.
- How platform permissions and data on the device are treated.
- What a person must be able to perceive, operate, and understand on a phone.

State the practice without ticket ids, environment names, credentials, or bundle identifiers.

## Stays in the project

- Requirements, copy, and visual design that exist for this product only.
- Environment names, credential locations, and bundle identifiers.
- Local architecture choices that depend on this product's backend, feature set, or release calendar.
- Test results that only make sense against this product's build.

Store submission and release automation stay in the CI/CD repo. A public HTTP API and other client-agnostic application rules stay in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).

## Promoting a project decision

A project decision can become a practice after it is rewritten so it still holds with that project's constraints removed, and after the check in [Verify on a mobile client, then record](04-verify-and-record.md) has been run. Until then it stays in the project.

Do not copy a project decision into this repo to make it feel official.

## Split lessons

When one effort produces a mobile lesson and a general application lesson, write the mobile lesson here and link to the application-development knowledge base for the general lesson. When it also produces an AI-tooling lesson, link to the [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base) for that lesson.
