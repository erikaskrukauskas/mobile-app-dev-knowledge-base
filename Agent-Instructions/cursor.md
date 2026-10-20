---
title: Cursor
tags: [agents, cursor]
status: verified
updated: 2026-10-19
---

# Cursor

Cursor reads this library when a project points at it. Product behavior for Cursor itself is documented in the [AI knowledge base](https://github.com/erikaskrukauskas/ai-knowledge-base), not here.

## This repo

`AGENTS.md` at the root tells agents how to maintain the library: mobile knowledge only, frontmatter, lesson status, and no secrets or copied manuals. Two project skills cover adding an uncovered mobile topic and reviewing topics this repo already documents.

## Other projects

Add the [consultation protocol](consultation-protocol.md) to the project's `AGENTS.md`. That file is the durable place for the search rule. A chat reminder disappears with the session.

Keep the protocol short. Link the practice pages instead of pasting them into the project.

## Search from a project

From any working directory:

```powershell
python "<path-to-mobile-app-dev-knowledge-base>\Search-Index\search.py" "navigation screen"
```

Phase 2 can replace that command with an MCP tool. Until [MCP-Server/README.md](../MCP-Server/README.md) is built, use the script.

## Agent behavior

Questions about how Cursor should brief, search, compare, verify, or record work are searched in the AI knowledge base. Mobile design questions are searched here. Application design questions that are not specific to a mobile client are searched in the [application-development knowledge base](https://github.com/erikaskrukauskas/app-dev-knowledge-base).
