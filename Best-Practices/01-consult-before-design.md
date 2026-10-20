---
title: Consult before a mobile design choice
tags: [practices, mobile, navigation, retrieval]
status: verified
updated: 2026-10-19
---

# Consult before a mobile design choice

Search this repository before a significant mobile design choice. Search the application-development knowledge base when the rule would still hold for a client that is not a phone. Search the AI knowledge base when the question is how an agent should work.

## Choose the library

| Question | Search |
| --- | --- |
| How should this mobile client be structured, navigated, contracted on screen, or checked on a device? | This repo |
| How should an application be structured, contracted, or checked when the answer does not depend on a mobile client? | [Application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base) |
| How should an agent brief, search, compare, verify, or record work? | [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base) |
| How should data be moved, modeled for analysis, released, or submitted to a store? | The data-engineering, data-science, or CI/CD repo |
| What did this product already decide? | That project's docs and history |

A new mobile project does not need a private copy of these practices. It needs a pointer to this checkout and a habit of searching it. The consultation snippet is in [Agent-Instructions/consultation-protocol.md](../Agent-Instructions/consultation-protocol.md).

## Sequence

1. Name the screen or platform behavior, the boundary, and the decision you are about to make. See [Specify the screen and done](02-specify-screen-and-done.md).
2. Search this repo for a mobile practice that applies: navigation, a screen contract, lifecycle, offline state, permissions, accessibility, or mobile security.
3. Search the application-development knowledge base when the open question is a general application rule, such as a public HTTP API or a security boundary any client could use.
4. Search the AI knowledge base only when the open question is about the agent's working method.
5. Read the current official documentation when the decision depends on a platform, an accessibility requirement, or a mobile test tool. See [Official-Documentation/README.md](../Official-Documentation/README.md). Confirm the current page before relying on a feature.
6. Name the real options, then implement one. See [Compare before choosing](03-compare-before-choosing.md).
7. Run the named check on a mobile client. See [Verify on a mobile client, then record](04-verify-and-record.md).
8. Write a reusable mobile lesson here. Write a general application lesson in the application-development knowledge base. Write an AI-tooling lesson in the AI knowledge base.

## What counts as significant

Search and compare when the work chooses app structure, navigation, a screen or UI contract, lifecycle behavior, where mobile state lives (including offline and local state), a mobile error-handling policy, a mobile accessibility commitment, or a device security boundary such as a platform permission.

A narrow local fix with an obvious edit can proceed from the code in front of you. Record a lesson afterward if the diagnosis would help another mobile client.

## Enforcement

The consultation protocol asks agents to do this. A project-start checklist is stronger because it is explicit. Use [Agent-Instructions/project-start-checklist.md](../Agent-Instructions/project-start-checklist.md) when a project should require the search.
