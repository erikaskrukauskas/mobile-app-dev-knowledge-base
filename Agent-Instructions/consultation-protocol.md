---
title: Consultation protocol
tags: [agents, mobile, retrieval]
status: verified
updated: 2026-10-19
---

# Consultation protocol

Paste this into a project's `AGENTS.md` or `CLAUDE.md`. Adjust the paths.

```markdown
## Knowledge bases

Mobile practices live in `<path-to-mobile-app-dev-knowledge-base>`.
Application practices that are not specific to a mobile client live in `<path-to-app-dev-knowledge-base>`.
AI working practices live in `<path-to-ai-knowledge-base>`.
Data engineering, data science, and CI/CD live in their own repos.
Project requirements, environment names, credentials, bundle identifiers, and local architecture choices stay in this project.

Before a significant change:

1. Mobile design questions are searched in `<path-to-mobile-app-dev-knowledge-base>`:
   `python "<path-to-mobile-app-dev-knowledge-base>\Search-Index\search.py" "<keywords>"`
2. Application design questions that are not specific to a mobile client are searched in `<path-to-app-dev-knowledge-base>`.
3. Questions about briefing, searching, comparing, verifying, or recording AI-assisted work are searched in `<path-to-ai-knowledge-base>`.
4. Data engineering, data science, and CI/CD questions go to those repos.
5. Significant design choices name the options, then implement one.
6. The named check is run before the work is called done.
7. A reusable mobile lesson is written in `<path-to-mobile-app-dev-knowledge-base>`. A general application lesson is written in `<path-to-app-dev-knowledge-base>`. An AI-tooling lesson is written in `<path-to-ai-knowledge-base>`.
```

Significant means app structure, navigation, a screen or UI contract, lifecycle, offline or local state, a platform permission, mobile accessibility, or mobile application security. A narrow local fix can proceed from the code at hand.

Apply a lesson only when its status is `verified` and its environment still matches. Confirm platform and accessibility behavior against current docs when a lesson and the docs disagree. See [Official-Documentation/README.md](../Official-Documentation/README.md).
