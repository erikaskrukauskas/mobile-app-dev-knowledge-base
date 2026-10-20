---
title: Mobile Application Development Knowledge Base
tags: [overview, mobile, scope]
status: verified
updated: 2026-10-19
---

# Mobile Application Development Knowledge Base

This repository is the shared library for **mobile-application knowledge**: app structure, navigation, screen and UI contracts, app lifecycle, offline and local state, platform permissions, mobile accessibility, mobile error handling, and mobile application security. Other projects consult it for practices that still apply after a single product's constraints are removed.

Application design that is not specific to a mobile client lives in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base). AI tooling lives in the [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base). Data engineering, data science, and CI/CD, including store submission and release automation, keep their own repositories. This repo stores how a mobile client is structured and checked.

## What belongs here

- Stable practices for mobile app structure, navigation, screen contracts, lifecycle, offline and local state, platform permissions, mobile accessibility, mobile error handling, and mobile application security.
- Lessons from real mobile work, after they have been checked on a mobile client.
- Pointers to current Apple platform docs, Android platform docs, mobile accessibility guidance, and mobile testing tools.
- Citations and original notes for mobile-application references. Full copyrighted books and PDFs stay out of git.

## How another project uses it

1. Point that project's agent instructions at this checkout. Copy the snippet from [Agent-Instructions/consultation-protocol.md](Agent-Instructions/consultation-protocol.md).
2. Search before a significant mobile design choice:

```powershell
python Search-Index/search.py "mobile accessibility"
python Search-Index/search.py --tag navigation
python Search-Index/search.py --list
```

3. Apply what is reusable. Leave requirements, environment names, credentials, bundle identifiers, and local architecture choices in the project repo.
4. After a checked mobile lesson, add a file under `Lessons-Learned/` using the template.

Questions about architecture, public HTTP APIs, shared state rules, and application security that any client could use belong in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base). On this machine that checkout is `C:\Users\erika\Cursor Projects\knowledge-base\app-dev-knowledge-base`.

Questions about briefing, searching, comparing, verifying, or recording AI-assisted work belong in the [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base). On this machine that checkout is `C:\Users\erika\Cursor Projects\knowledge-base\ai-knowledge-base`.

## Layout

| Path | Role |
| --- | --- |
| `Best-Practices/` | Stable mobile-application practices |
| `Lessons-Learned/` | Findings from real mobile work and their validation state |
| `Agent-Instructions/` | Pointers for Cursor, Codex, Claude Code, and ChatGPT |
| `Official-Documentation/` | Links to current Apple, Android, accessibility, and mobile testing docs |
| `Books/` | Citation and notes policy for references |
| `Search-Index/` | Local keyword search over this repo |
| `MCP-Server/` | Design for a later shared retrieval service |
| `AGENTS.md` | Rules for agents editing this repo |
| `SCOPE.md` | Boundary between this repo and sibling repos |

## Roadmap

| Phase | Outcome | State |
| --- | --- | --- |
| 1. Foundation | Folder layout, practices, lessons template, keyword search | In this repo |
| 2. MCP | Local MCP tools so agents can search from any project | Designed, not built |
| 3. Lessons memory | Validation workflow, superseding, retrieval of verified lessons | Template and rules are in place |
| 4. Remote access | Authenticated API or connector for agents that cannot read a local checkout | Later, after a local workflow is proven |

## Principles

- Search this repo for a mobile design question. Search the application-development knowledge base for a general application rule. Search the AI knowledge base for how an agent should work.
- Record a lesson after a test or an exercised user path on a mobile client. Mark replacements as superseded.
- Keep one copy of each practice. Agent-specific files link to it.
- Keep a product's requirements, credentials, bundle identifiers, and local choices in that project.
