---
id: LL-0001
title: Keep this repo to mobile application development
tags: [lessons, scope, governance, mobile]
status: verified
updated: 2026-10-19
environment: "Cursor, Windows, mobile-app-dev-knowledge-base repo"
scope: global
superseded_by:
---

# Keep this repo to mobile application development

## Problem

Mobile client design, general application design, agent workflow, data work, and release automation were easy to store in one library. A search in that library would return a prompting habit next to a screen contract, and a later project could treat a product-specific bundle identifier as a general mobile rule.

## Approaches that failed

- Approach: Plan one engineering library that holds mobile clients, general application design, AI tooling, data engineering, data science, and CI/CD.
- Why it failed: Each of those subjects has its own repo. Mixing them makes search results noisier and encourages an agent to apply a public HTTP rule, a data-pipeline decision, or a store-release step as if it were a mobile practice.
- Evidence: Scope decision for this repository, 2026-10-19.

## Working solution

Use this repository only for mobile-application knowledge: app structure, navigation, screen and UI contracts, app lifecycle, offline and local state, platform permissions, mobile accessibility, mobile error handling, and mobile application security.

Put general architecture, public HTTP APIs, shared state rules, and application security that any client could use in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base). Put agent briefing, retrieval, and lesson-capture method in the [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base). Put data engineering, data science, and CI/CD, including store submission and release automation, in their own repos. Put requirements, environment names, credentials, bundle identifiers, and local architecture choices in the project.

When one effort produces both a mobile lesson and a general application lesson, write the mobile lesson here and link to the application-development knowledge base for the general lesson. When it also produces an AI-tooling lesson, link to the AI knowledge base for that lesson. See [SCOPE.md](../SCOPE.md).

## Verification

- Check run: Scope review against the repository decision and the folder layout on 2026-10-19.
- Result: Root docs and best-practice pages describe mobile client design and checks. General application rules, agent workflow, data platforms, and release automation appear as subjects that belong in other repos.

## Scope

`global` for any future project that consults this knowledge base.

## References

- [SCOPE.md](../SCOPE.md)
- [Practice versus project](../Best-Practices/05-practice-versus-project.md)
