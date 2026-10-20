---
title: Scope of this repository
tags: [scope, governance, mobile]
status: verified
updated: 2026-10-19
---

# Scope

This repository is the mobile-application knowledge base. Other projects read it for practices and verified lessons about building a mobile client that a future mobile project can reuse.

## In this repo

- App structure that still applies after one product's constraints are removed.
- Navigation, screen and UI contracts, and the boundary between screens.
- App lifecycle: what the mobile client does when it starts, backgrounds, resumes, and stops.
- Offline and local state: what the device keeps, and how the client behaves when the network is absent.
- Platform permissions, data stored on the device, and secrets kept out of git.
- Mobile accessibility: what a person must be able to perceive, operate, and understand on a phone.
- Mobile error handling: what the person on the device sees when a screen, a permission, or a local store fails.
- Mobile application security that depends on the device, the permission model, or data that stays on the phone.

A platform or a framework is not the practice. iOS, Android, and a cross-platform toolkit belong on an [official-doc pointer](Official-Documentation/README.md). Practices stay useful for a native app and for a cross-platform app.

## In other repos

| Topic | Where it lives |
| --- | --- |
| Application design that is not specific to a mobile client: general architecture, public HTTP APIs, shared state rules, and application security any client could use | [Application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base) |
| AI tooling, agent instructions, prompting, retrieval, and MCP | [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base) |
| Data engineering | Its own knowledge repo |
| Data science | Its own knowledge repo |
| CI/CD, store submission, and release automation | Its own knowledge repo |
| A single project's requirements, environment names, credentials, bundle identifiers, and local architecture choices | That project |

On this machine the application-development checkout is `C:\Users\erika\Cursor Projects\knowledge-base\app-dev-knowledge-base`. The AI knowledge base checkout is `C:\Users\erika\Cursor Projects\knowledge-base\ai-knowledge-base`.

A lesson about a public HTTP contract, an agent workflow, a warehouse model, a statistical method, or a store release is recorded in the matching repo. If that work also produced a reusable mobile lesson (for example, a clearer screen contract or a permission check on the device), write the mobile lesson here and link to the other write-up.

## Where a new note goes

Ask what a future mobile project in an unrelated product could reuse.

- If the answer is how to structure, navigate, contract, or check a mobile client, add it here.
- If the answer is how to shape, contract, or check an application without depending on a mobile client, add it to the application-development knowledge base.
- If the answer is how an agent should brief, search, compare, verify, or record work, add it to the AI knowledge base.
- If the answer depends on a dataset, a model, a release system, or store submission, add it to that domain repo.
- If the answer only makes sense with this product's requirements, environment names, credentials, or bundle identifiers, keep it in the project.
- If one effort produces both a mobile lesson and a general application lesson, write the mobile lesson here and link to the application-development knowledge base for the general lesson. If it also produces an AI-tooling lesson, link to the AI knowledge base for that lesson.

## Reusable practice and project knowledge

Reusable practice in this repo applies across mobile projects: how to specify a screen, how to compare navigation options, how to treat data on the device.

Project knowledge stays in the project: requirements, environment names, credential locations, bundle identifiers, local architecture choices, and test results that only make sense there.

Do not copy a project decision into this repo to make it feel official. Promote it only after it is stated as a practice that still holds without that project's constraints.
