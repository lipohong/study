# Jekyll Learning Archive

This is a bilingual, Jekyll-first archive for deliberate practice and self-directed learning. Every learning record is a post, so the website is the library rather than a separate export of local folders.

## Start here

1. Read [AGENTS.md](AGENTS.md) for the rules agents must follow.
2. Open the website's **Categories**, **Tags**, and **Archives** tabs to browse the library.
3. Read the current-goal and learner-context posts before starting a learning session.

## Content library

All learning Markdown lives in `_posts/<record-type>/`. Each post has one top-level category that identifies its role and powers the Jekyll category view.

| Category | What it contains |
|---|---|
| `goals` | Active goal, long-term goal, and breakdown |
| `learner-context` | Learner profile and current learning state |
| `knowledge` | Reusable concepts, models, explanations, and diagrams |
| `ideas`, `thinking`, `reflections` | Captures, learner reasoning, and reflection |
| `drills`, `attempts`, `feedback`, `scorecards` | Deliberate-practice evidence |
| `sources` | Source records and citation notes |
| `logs`, `reviews` | Chronological session history and synthesis |
| `templates` | Reusable post structures |

Each English canonical post has a Chinese partner beside it:

```text
_posts/knowledge/2026-09-17-topic.md
_posts/knowledge/2026-09-17-topic.zh-CN.md
```

Posts use explicit English and Chinese permalinks, stable categories, and narrow topic tags. Link posts by permalink and link visual assets from `/Diagrams/`; do not use relative links to old workspace folders.

## Creating a record

Create the English and Chinese posts together in the matching record-type folder. Use the required front matter documented in `AGENTS.md`: title, date, permalink, categories, tags, description, comments, table-of-contents setting, language, translation key, and record type.

The repository is public-site content by design. Do not place credentials, private tokens, sensitive personal data, or unapproved copyrighted transcripts in a post.

## Technical files

The root contains only the operational files the site needs: agent instructions, this guide, Jekyll configuration, dependencies, deployment workflow, site tabs, plugins, assets, and diagrams. Learning documents do not belong in separate root-level content folders.
