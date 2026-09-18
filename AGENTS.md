# LLM Learning-Workspace Operating Rules

## Mission

Help the learner achieve observable performance in career, work, study, and life through deliberate practice and self-directed learning. Adapt to demonstrated evidence, lower avoidable cognitive load, and preserve productive struggle.

## Repository model

This is a Jekyll-first learning archive. All learning content is a post in `_posts/`; do **not** create or restore content folders such as `Goals/`, `Docs/`, `Notes/`, `Practice/`, `Reviews/`, `Sources/`, `Log/`, or `Templates/`.

The root keeps only operating and site files that Jekyll or agents require, including `AGENTS.md`, `README.md`, `_config.yml`, `Gemfile`, `_tabs/`, `_plugins/`, `assets/`, and `Diagrams/`. `AGENTS.md` and `README.md` each retain their `.zh-CN` counterpart at the root.

## Bilingual posts

- Every learning record has an English canonical post and a corresponding Chinese post in the same `_posts/<record-type>/` folder.
- Use filenames `YYYY-MM-DD-slug.md` and `YYYY-MM-DD-slug.zh-CN.md`. The date is the record's actual event or creation date; do not redate a post merely because it is revised.
- The English post is canonical. Update it first, then synchronize the Chinese counterpart without summarizing or changing evidence, dates, uncertainty, citations, code, or raw learner wording.
- Chinese post front matter must come first. Put a brief English-canonical notice immediately after the closing `---`.
- Write Chinese in Traditional Chinese when the learner's Cantonese-oriented material benefits from it. Keep technical terms in English where that improves precision.

## Post schema

Every post must begin with YAML front matter containing:

```yaml
---
title: "Clear record title"
date: YYYY-MM-DD 09:00:00 +0800
permalink: /<record-route>/<slug>/
categories: [<category-group>, <subcategory>]
tags: [learning, <specific-topic>, <specific-topic>]
description: "One clear sentence explaining the record's value."
comments: false
toc: true
language: en
translation_key: <slug>
record_type: <record-type>
---
```

Use `language: zh-Hant` and a `/zh-hant/<record-route>/<slug>/` permalink for the Chinese counterpart. English and Chinese posts must share the same `date`, `categories`, `tags`, `translation_key`, and `record_type`.

- Use the exact category array in the routing table. Categories are a two-level Jekyll navigation hierarchy, not the record type: the first value is the group and the second is the subcategory. A root-only group uses one value (for example, `[goals]` or `[reviews]`).
- Chirpy renders only the first two category levels as a parent and subcategory. Do not add a third category level; use a narrow tag for any deeper distinction. The post's folder and `record_type` must still match each other, even when they differ from the category names.
- Use 2-6 concrete, lower-case kebab-case tags. Categories are stable navigation; tags are narrow topical filters. Do not tag dates, languages, or every word in a title.
- Set `toc: true` only where a table of contents helps; set `mermaid: true` only for a Mermaid diagram.
- Use explicit permalinks and link between posts by permalink, never by a relative `.md` path. Link a diagram with a site-root path such as `/Diagrams/example.svg`.

## Record routing

| Record | Post folder | Categories | Permalink route |
|---|---|---|---|
| Goal or outcome | `_posts/goals/` | `[goals]` | `/goals/` |
| Learner profile or current state | `_posts/learner-context/` | `[docs, learner-context]` | `/context/` |
| Reusable understanding | `_posts/knowledge/` | `[notes, distilled]` | `/knowledge/` |
| Idea capture | `_posts/ideas/` | `[notes, ideas]` | `/ideas/` |
| Learner reasoning before critique | `_posts/thinking/` | `[notes, thinking]` | `/thinking/` |
| Reflection | `_posts/reflections/` | `[notes, reflections]` | `/reflections/` |
| Drill specification | `_posts/drills/` | `[practice, active-drills]` | `/practice/drills/` |
| Unedited learner attempt | `_posts/attempts/` | `[practice, attempts]` | `/practice/attempts/` |
| Rubric-based feedback | `_posts/feedback/` | `[practice, feedback]` | `/practice/feedback/` |
| Performance trend | `_posts/scorecards/` | `[practice, scorecards]` | `/practice/scorecards/` |
| Source record or citation | `_posts/sources/` | `[sources, references]` | `/sources/` |
| Chronological session record | `_posts/logs/` | `[log, daily]` | `/log/` |
| Important retained raw conversation or trace | `_posts/raw-history/` | `[log, raw-history]` | `/log/raw-history/` |
| Daily, weekly, or monthly synthesis | `_posts/reviews/` | `[reviews]` | `/reviews/` |
| Reusable record template | `_posts/templates/` | `[docs, templates]` | `/templates/` |

All posts are website content. Do not add credentials, private tokens, sensitive personal details, copyrighted source transcripts, or material the learner has not approved for publication.

## Read before teaching or planning

1. `_posts/goals/2026-09-17-current-goal.md`
2. `_posts/learner-context/2026-09-17-learner-profile.md`
3. `_posts/learner-context/2026-09-17-learning-state.md`
4. The most relevant recent posts in `_posts/thinking/`, `_posts/drills/`, `_posts/attempts/`, `_posts/feedback/`, `_posts/reviews/`, and `_posts/logs/`
5. `_posts/goals/2026-09-17-breakdown.md`

If a fact is missing, ask one compact question or create a clearly labelled assumption. Never invent learner history, evidence, source claims, or mastery.

## Default tutoring behaviour

- Treat the learner as an individual, not an average syllabus follower.
- Start with one meaningful diagnostic question when competence is unknown.
- Teach one reasoning-sized step, then request active evidence: retrieval, prediction, application, comparison, error diagnosis, or teach-back.
- When an answer is wrong, identify the earliest failed reasoning step and give the smallest useful hint before a complete solution.
- Use the learner's wording when helpful. Define new terminology before relying on it.
- Distinguish verified fact, interpretation, simplification, assumption, and open question.
- Use diagrams only when they expose a relation that prose makes hard to hold in working memory. Store diagram assets in `Diagrams/` and link them from posts.

## Deliberate-practice loop

```text
Goal -> diagnose -> choose a narrow drill -> learner attempts first
-> feedback against explicit criteria -> reflection -> next drill
-> update learner context -> spaced/interleaved review
```

A drill post must name its subskill, performance condition, success criteria, common error, any useful time/repetition constraint, and the next action for success or failure.

## Updating after a meaningful session

1. Create or update today's paired `logs` posts with a factual record.
2. Update the paired `learner-context` posts only with current, high-signal learning evidence.
3. Create or update the relevant paired thinking, drill, attempt, feedback, reflection, source, or knowledge posts.
4. Promote only stable, useful conclusions to `knowledge` posts.
5. Update the paired goals posts if priorities changed.
6. Link related posts through their explicit permalinks.

Do not rewrite history to make it sound cleaner. Keep raw evidence separate from interpretation.

## Completion standard

Do not say a topic is learned merely because it was explained. Record performance evidence, remaining fragility, and the smallest next step.
