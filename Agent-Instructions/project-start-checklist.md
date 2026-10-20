---
title: Project-start checklist
tags: [agents, mobile, testing]
status: verified
updated: 2026-10-19
---

# Project-start checklist

The consultation protocol states the rule. This checklist is the stronger version: run it at the start of a project and again before a large mobile change.

## Checklist

- [ ] Project agent instructions include the [consultation protocol](consultation-protocol.md) and the correct path to this repo.
- [ ] The application-development knowledge base is linked for rules that are not specific to a mobile client.
- [ ] The AI knowledge base is linked for questions about how an agent should work.
- [ ] Data engineering, data science, and CI/CD repos are linked from the project when this work depends on them.
- [ ] Searched this repo for practices that match the design (`navigation`, `lifecycle`, `offline`, `permissions`, `accessibility`, `security`, `screen`, or `state`).
- [ ] Searched `Lessons-Learned/` for verified lessons in a similar device environment.
- [ ] Named the screen or platform behavior, the boundary, and the check that defines done.
- [ ] For a significant design, named the real options before implementing one.
- [ ] Confirmed platform, accessibility, or mobile-testing behavior that the design depends on, using current official docs.

## After the work

- [ ] The named check was run on a mobile client: a test, an exercised user path, or both.
- [ ] A reusable mobile lesson was added here only if a later mobile project would otherwise repeat the same investigation.
- [ ] A general application lesson, if any, was written in the application-development knowledge base and linked.
- [ ] An AI-tooling lesson, if any, was written in the AI knowledge base and linked.
- [ ] No secrets, environment credentials, bundle identifiers, or copyrighted sources were copied into this repo.

## Where the notes go

Mobile design stays in this repo. General application design stays in the application-development knowledge base. Agent method stays in the AI knowledge base. A single product's requirements stay in the project. See [Practice versus project](../Best-Practices/05-practice-versus-project.md).
