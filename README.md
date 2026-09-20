# AI Prompt Engineering

A public library of reusable AI prompts — browse by category, copy what you need, and contribute your own.

Maintained by [Joel Merciadez](https://github.com/joelmerciadez) ([Bytes & Bites](https://github.com/joelmerciadez)).

## Browse

Prompts live under [`prompts/`](prompts/), grouped by category:

| Category | Path | Best for |
| --- | --- | --- |
| Coding | [`prompts/coding/`](prompts/coding/) | Reviews, refactors, debugging, tests |
| Writing | [`prompts/writing/`](prompts/writing/) | Outlines, edits, tone, drafts |
| Research | [`prompts/research/`](prompts/research/) | Summaries, comparisons, source checks |
| Productivity | [`prompts/productivity/`](prompts/productivity/) | Planning, prioritization, workflows |
| Image | [`prompts/image/`](prompts/image/) | Image / visual generation prompts |
| Agents | [`prompts/agents/`](prompts/agents/) | Multi-step agent instructions |

Curated sets (optional playlists of prompts) live in [`collections/`](collections/).

Tag and category vocabulary is documented in [`meta/taxonomy.md`](meta/taxonomy.md).

## Use a prompt

1. Open a markdown file in `prompts/<category>/`.
2. Read the YAML frontmatter for title, tags, and model hints.
3. Copy the prompt body into your AI tool of choice.
4. Replace any `{{placeholders}}` with your own inputs.

Files marked **example** or **sample** in the frontmatter (or filename) are starter illustrations — not necessarily Joel’s personal production prompts.

## Contribute

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for filename rules, frontmatter fields, and the pull-request flow.

Quick start: copy [`templates/prompt.md`](templates/prompt.md) into the right category folder, fill it in, and open a PR.

## License

MIT — see [`LICENSE`](LICENSE).
