# Jekyll Learning Archive

This is a bilingual, Jekyll-first archive for deliberate practice and self-directed learning. Every learning record is a post, so the website is the library rather than a separate export of local folders.

## Start here

1. Read [AGENTS.md](AGENTS.md) for the rules agents must follow.
2. Open the website's **Categories** and **Tags** tabs to browse the library.
3. Read the current-goal and learner-context posts before starting a learning session.

## Content library

All learning Markdown lives in `_posts/<record-type>/`. Post folders and `record_type` identify the kind of record; `categories` provide the compact, two-level navigation shown on the Jekyll Categories page. The first category is the group and the second is its subcategory. Do not add a third category level; use tags for finer distinctions.

| Category group | Subcategories | Record types / folders |
|---|---|---|
| `goals` | — | Goals and outcomes: `_posts/goals/` |
| `notes` | `ideas`, `thinking`, `reflections`, `distilled` | Captures, learner reasoning, reflections, and reusable knowledge: `_posts/ideas/`, `_posts/thinking/`, `_posts/reflections/`, `_posts/knowledge/` |
| `practice` | `active-drills`, `attempts`, `feedback`, `scorecards` | Deliberate-practice specifications and evidence: `_posts/drills/`, `_posts/attempts/`, `_posts/feedback/`, `_posts/scorecards/` |
| `docs` | `learner-context`, `templates` | Learner profile/current state and reusable record structures: `_posts/learner-context/`, `_posts/templates/` |
| `sources` | `references` | Source records, citation notes, and approved reference materials: `_posts/sources/` |
| `log` | `daily`, `raw-history` | Daily session records and deliberately retained raw traces: `_posts/logs/`, `_posts/raw-history/` |
| `reviews` | — | Daily, weekly, or monthly synthesis: `_posts/reviews/` |

Each English canonical post has a Chinese partner beside it:

```text
_posts/knowledge/2026-09-17-topic.md
_posts/knowledge/2026-09-17-topic.zh-CN.md
```

Posts use explicit English and Chinese permalinks, the routing-table category hierarchy, and narrow topic tags. Link posts by permalink and link visual assets from `/Diagrams/`; do not use relative links to old workspace folders.

## Creating a record

Create the English and Chinese posts together in the matching record-type folder. Use the required front matter documented in `AGENTS.md`: title, date, permalink, categories, tags, description, comments, table-of-contents setting, language, translation key, and record type.

The repository is public-site content by design. Do not place credentials, private tokens, sensitive personal data, or unapproved copyrighted transcripts in a post.

## Technical files

The root contains only the operational files the site needs: agent instructions, this guide, Jekyll configuration, dependencies, deployment workflow, site tabs, plugins, assets, and diagrams. Learning documents do not belong in separate root-level content folders.
