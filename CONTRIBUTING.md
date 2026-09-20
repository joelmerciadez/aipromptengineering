# Contributing

Thanks for helping grow this prompt library. Keep contributions small, reusable, and clearly labeled.

## Add a prompt

1. Copy [`templates/prompt.md`](templates/prompt.md).
2. Place it under the best category folder:

   - `prompts/coding/`
   - `prompts/writing/`
   - `prompts/research/`
   - `prompts/productivity/`
   - `prompts/image/`
   - `prompts/agents/`

3. Name the file with kebab-case: `code-review-checklist.md`, `meeting-notes-summary.md`.
4. Fill in the YAML frontmatter (required fields below).
5. Write the prompt body. Prefer clear sections and `{{placeholders}}` for user inputs.
6. Open a pull request against `main`.

If you are unsure of the category, pick the closest fit and note alternatives in the PR description. See [`meta/taxonomy.md`](meta/taxonomy.md) for tags.

## Filename rules

- Lowercase kebab-case only: `a-z`, `0-9`, and `-`
- End with `.md`
- Prefer a verb or outcome in the name (`debug-failing-test`, `tighten-blog-draft`)
- Prefix with `example-` only for sample/demo prompts that are not claimed as the author’s production set

## Frontmatter

```yaml
---
title: Short human title
description: One sentence on when to use this prompt
tags: [coding, review]
models: [gpt-4o, claude-sonnet]
author: your-github-username
example: false
---
```

| Field | Required | Notes |
| --- | --- | --- |
| `title` | yes | Display name |
| `description` | yes | One sentence |
| `tags` | yes | From [`meta/taxonomy.md`](meta/taxonomy.md); add new tags only when needed |
| `models` | no | Suggested models / families; omit if model-agnostic |
| `author` | yes | GitHub username or `example` for samples |
| `example` | no | Set `true` for sample/demo prompts |

## Prompt body guidelines

- Lead with role or goal when it helps.
- List constraints and output format explicitly.
- Use `{{variable_name}}` for inputs the user must supply.
- Avoid private data, credentials, or unpublished client content.
- Do not present sample prompts as Joel’s personal prompts unless he authored them.

## Collections

To group related prompts, add a folder under `collections/` with a short `README.md` that links to the prompt files (do not duplicate the full prompt text).

## Pull requests

- One prompt (or one tightly related set) per PR when possible
- Describe what the prompt is for and how you tested it
- Confirm the frontmatter validates against the table above
