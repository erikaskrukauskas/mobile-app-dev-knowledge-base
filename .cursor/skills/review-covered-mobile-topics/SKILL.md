---
name: review-covered-mobile-topics
description: >-
  Review official Apple, Android, mobile accessibility, and mobile testing
  sources for changes to mobile topics this knowledge base already documents,
  then update those pages. Use when the user asks to review covered topics,
  refresh existing practices against current documentation, or check whether
  documented mobile guidance is outdated.
---

# Review covered mobile topics

Start from the pages already in this repo. Check whether current sources still agree with them. This is not a search for new topics. New topics use [add-uncovered-mobile-topic](../add-uncovered-mobile-topic/SKILL.md).

Do not commit or push unless the user asks.

## List the covered topics

```bash
python Search-Index/search.py --list
```

Review `Best-Practices/`, verified files in `Lessons-Learned/`, and claims in `Official-Documentation/` and `Books/`. Skip `Lessons-Learned/_template.md`, files with `status: superseded`, files under `.cursor/`, and files in `Official-Documentation/updates/`.

For each remaining page, note the claim a current source could invalidate: a platform permission, an accessibility requirement, a lifecycle default, a cited URL, or a behavior presented as current. Skip a page that states a stack-neutral rule with no source claim.

## Check sources for those claims

Start with the URL cited on the page. If the page has no URL, use the matching entry in [Official-Documentation/README.md](../../../Official-Documentation/README.md). Open the current page with WebFetch or WebSearch and read the section that matches the claim. Confirm that page before treating a feature as current.

A blog or community post is a lead. It does not change a practice until an official page confirms it.

Leave general application-design changes to the application-development knowledge base. Leave agent-product changes (Cursor, Codex, Claude, ChatGPT, MCP client behavior) to the AI knowledge base. Leave data-platform, store-submission, and release-tool changes to those repos.

A source that does not touch a covered claim is out of this review.

## Update the page

Edit the existing page when an official source contradicts or narrows that claim. Set `updated` to the day you check it. Keep `status` unless the page is wrong enough to replace. A replacement gets a new page; the old page becomes `superseded` and its `superseded_by` points at the replacement. Do not delete it.

When you recheck the entry points, set the checked date in `Official-Documentation/README.md`.

Do not add a new topic during this review. Do not paste a manual or book into the repo. Quote only the sentence needed, with the URL.

A doc change is not a lesson. Add a lesson only when a mobile client in this environment was checked against the change.

## Report

Write `Official-Documentation/updates/YYYY-MM-DD-covered-topics.md` with frontmatter `title`, `tags: [documentation, updates]`, `status: verified`, and `updated`. Put the same report in the chat:

```markdown
# Covered topic review
Checked: YYYY-MM-DD

## Updated
- **Page** — what the source changed — [url](url)

## Still current
- Page — source checked

## Unconfirmed
- Page — claim that could not be checked, and which source failed
```
