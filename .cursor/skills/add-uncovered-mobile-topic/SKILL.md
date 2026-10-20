---
name: add-uncovered-mobile-topic
description: >-
  Add a missing mobile-application topic to this knowledge base after
  confirming no page covers it. Use when the user asks to document, add, or
  update this knowledge base on a topic it does not yet cover, including app
  structure, navigation, screen or UI contracts, app lifecycle, offline and
  local state, platform permissions, mobile accessibility, mobile error
  handling, or mobile application security.
---

# Add an uncovered mobile topic

Add one new mobile-application topic. If a page already answers it, edit that page. Refreshing a covered page from current sources uses [review-covered-mobile-topics](../review-covered-mobile-topics/SKILL.md).

Do not commit or push unless the user asks.

## Decide where it goes

Read [SCOPE.md](../../../SCOPE.md). Add the topic here only when a future mobile project in an unrelated product could reuse it.

Stop and name the other home when the topic is:

- Application design that is not specific to a mobile client: the application-development knowledge base
- How an agent should brief, search, compare, verify, or record work: the AI knowledge base
- Data engineering, data science, or CI/CD, including store submission and release automation: that repo
- One product's requirements, environment names, credentials, bundle identifiers, or local architecture: that project

A platform or a framework is not the practice. Put it on an official-doc pointer.

## Confirm it is uncovered

From the repo root:

```bash
python Search-Index/search.py --list
python Search-Index/search.py "topic words"
```

Search `Best-Practices/`, `Lessons-Learned/`, `Official-Documentation/`, `Agent-Instructions/`, and `Books/`. Ignore hits under `.cursor/`.

A page that answers the question means the topic is covered. Edit that page, or follow [review-covered-mobile-topics](../review-covered-mobile-topics/SKILL.md) when the task is to refresh it.

A near match is still covered when the missing part is a paragraph, not a new decision. Add the paragraph there.

## Research before writing

Open the current official page with WebSearch or WebFetch. Start from [Official-Documentation/README.md](../../../Official-Documentation/README.md), then open the section that supports the rule. Confirm that page before relying on a feature.

A blog or community post is a lead. Confirm it on an official page before writing it as a practice.

Quote only the sentence needed, with the URL. Do not paste a manual, a book chapter, or a secret.

Stay stack-neutral. A framework, language, or platform belongs on an official-doc pointer, not as the practice itself.

## Write one page

Follow [Write findable pages](../../../Best-Practices/08-write-findable-pages.md).

| Kind of knowledge | Where to put it |
| --- | --- |
| Stable rule another mobile project can apply | Next numbered file in `Best-Practices/`, plus a row in its README |
| Pointer to current Apple, Android, accessibility, or mobile testing docs | A row or a short note under `Official-Documentation/` |
| Citation and original notes for a book | A catalog row and `Books/notes/<slug>.md` |
| Finding from a checked change on a mobile client | Next `LL-####` file, using `Lessons-Learned/_template.md` |

One topic per page. Link the canonical page instead of copying it. A general application rule links to the application-development knowledge base instead of being restated. Tags are lowercase search words. Set `updated` to the day you write the page.

Status:

- `candidate` when the only support is an unconfirmed lead
- `tested` when you opened the current official page and the new page states the rule with that URL and the date checked
- `verified` only when the check named on the page was run, or the user explicitly asks for `verified`

Do not mark a lesson `verified` unless that check was run. A new lesson starts as `candidate` or `tested`.

## Finish

Search the words a later project would type and confirm the new page hits. Update the index README for the folder you changed.

```markdown
# Topic added
- Page:
- Why it was uncovered:
- Primary source: [title](url)
- Status:
```

If you refused the topic, say where it belongs.
