---
title: Codex
tags: [agents, codex]
status: verified
updated: 2026-10-19
---

# Codex

Codex should use the same mobile library as Cursor and Claude Code. Product behavior for Codex itself is documented in the [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base), not here.

## Instructions

Include the [consultation protocol](consultation-protocol.md) in the global agent instructions so a new project inherits the search habit. Use the project's own instructions for constraints that are true only in that repository.

Add the [project-start checklist](project-start-checklist.md) when a project should require the search at kickoff.

## What Codex reads

- This repo for app structure, navigation, screen contracts, lifecycle, offline and local state, platform permissions, mobile accessibility, mobile error handling, and mobile application security.
- The [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base) for rules that are not specific to a mobile client.
- The AI knowledge base for how to brief, search, compare, verify, and record AI-assisted work.
- The project for requirements, environment names, bundle identifiers, and local decisions.

Codex should not copy this repo into each project.

## MCP

When the local MCP server from [MCP-Server/README.md](../MCP-Server/README.md) exists, register it in the Codex configuration. Until then, run `Search-Index/search.py`.
