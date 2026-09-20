# Prompt template

Copy this file into `prompts/<category>/your-prompt-name.md`, then replace the placeholders.

```markdown
---
title: Your prompt title
description: One sentence describing when to use this prompt
tags: [category-tag]
models: []
author: your-github-username
example: false
---

# Instructions

You are {{role}}. Your goal is to {{goal}}.

## Context

{{context}}

## Constraints

- {{constraint_1}}
- {{constraint_2}}

## Output format

{{output_format}}

## Input

{{user_input}}
```

Tips:

- Keep the frontmatter accurate so others can search by tag.
- Prefer explicit output structure (headings, bullets, tables) over vague “be helpful” instructions.
- Mark `example: true` and set `author: example` for sample/demo prompts.
