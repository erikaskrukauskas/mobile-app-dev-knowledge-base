---
title: Agent rules for this repository
tags: [agents, governance]
status: verified
updated: 2026-10-19
---

# Agent rules

You are in the mobile-application knowledge base. Other projects consult this repo for app structure, navigation, screen and UI contracts, app lifecycle, offline and local state, platform permissions, mobile accessibility, mobile error handling, and mobile application security. General application design, AI tooling, data engineering, data science, and CI/CD have their own repos.

## While editing this repo

- Add or update mobile-application knowledge only. Read [SCOPE.md](SCOPE.md) before creating a document.
- Put stable guidance in `Best-Practices/`. Put findings from real work in `Lessons-Learned/`.
- Give every document YAML frontmatter with `title`, `tags`, `status`, and `updated`.
- Lessons also have `id`, `environment`, `scope`, and `superseded_by`.
- Keep one canonical copy of a practice. Link to it from agent-specific files.
- Do not commit secrets, credentials, copyrighted books, or verbatim official documentation.
- Do not present an untested finding as `verified`. Use the lifecycle in [Lessons-Learned/README.md](Lessons-Learned/README.md).
- When a newer document replaces an older one, set the old document to `superseded` and point `superseded_by` at the replacement. Do not delete it.
- Do not commit or push unless the task explicitly asks for that.

## Status values

`candidate` → `tested` → `verified`

Use `superseded` when a newer document replaces this one. Keep the old file so past references still resolve.

## Questions that belong elsewhere

- Application design that is not specific to a mobile client: the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).
- How an agent should brief, search, compare, verify, or record work: the [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base).
- Data engineering, data science, and CI/CD, including store submission and release automation: those repos.
- One product's requirements, environment names, credentials, bundle identifiers, and local architecture choices: that project.

## Skills

- A topic this repo does not yet cover: `.cursor/skills/add-uncovered-mobile-topic/SKILL.md`
- Whether a covered topic still matches current sources: `.cursor/skills/review-covered-mobile-topics/SKILL.md`

Hits under `.cursor/` do not mean a topic is covered.

## Before you finish a documentation change

Search for an existing page on the same topic:

```powershell
python Search-Index/search.py --list
python Search-Index/search.py "your topic"
```

Update the existing page when the topic already exists.
