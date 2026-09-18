---
title: "Practice Drill Template"
date: 2026-09-17 09:00:00 +0800
permalink: /templates/practice-drill/
categories: [templates]
tags: [learning, template, workspace]
description: "templates record: Practice Drill Template."
comments: false
toc: true
language: en
translation_key: templates-practice-drill
record_type: templates
---

> **Chinese version:** [/zh-hant/templates/practice-drill/](/zh-hant/templates/practice-drill/)

## Reusable template

```markdown

## Drill

- **Skill / subskill:**
- **Why this drill:**
- **Starting level:** secure / fragile / missing / unknown
- **Timebox / repetitions:**

## Performance condition

Describe the task exactly as it should be attempted. Include realistic constraints, allowed tools, and what must be done without help.

## Success criteria

- [ ]
- [ ]
- [ ]

## Common error to watch

-

## Attempt instructions

1. Attempt first without receiving the final answer.
2. Save the unedited work under `Practice/Attempts/`.
3. Request feedback against the success criteria.
4. Write the smallest useful correction in a reflection note.

## LLM coach prompt

> Act as a deliberate-practice coach. Do not solve this task before I attempt it. First confirm the performance condition and success criteria. After my attempt, identify the earliest reasoning or execution failure, give one minimal hint, let me retry, then provide a rubric-based review. Update the recommended next drill based on my evidence.

## Next-step rule

- If successful with explanation: increase variation, speed, or realism.
- If partly successful: repeat with one reduced source of difficulty.
- If unsuccessful: identify and practise the missing prerequisite.

```