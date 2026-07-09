# agent-skills

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Agent Skills](https://img.shields.io/badge/format-Agent%20Skills-b083f0)](https://code.claude.com/docs/en/skills)

A collection of [Agent Skills](https://code.claude.com/docs/en/skills) for Claude Code and other coding agents. Same `SKILL.md` files also work in Claude Desktop, Codex CLI, ChatGPT, Gemini CLI, and other tools that speak the open Agent Skills format.

## Install

```bash
npx skills add warstellar/agent-skills
```

Or install a single skill directly:

```bash
npx skills add warstellar/agent-skills --skill deslop
```

Check the CLI's docs for the full syntax (`npx skills --help`).

## Skills

- **[deslop](skills/deslop/SKILL.md)** — detects, critiques, and rewrites text to remove AI writing patterns (word choice, rhythm, structural tells) so it reads like a specific, thoughtful human wrote it.

  <details>
  <summary>Example</summary>

  | AI version | Human version |
  |---|---|
  | "This isn't just a tool. It's a revolution." | "This tool cut onboarding from 3 weeks to 4 days." |
  | "serves as a critical component, ensuring seamless integration" | "is the piece that connects the two systems" |

  </details>

## Adding a new skill

Each skill lives in its own folder under `skills/`:

```
skills/<skill-name>/SKILL.md
```

`SKILL.md` must start with YAML frontmatter containing `name` and `description`.

## License

[MIT](LICENSE)

## Author

Ian Corvin — [github.com/warstellar](https://github.com/warstellar)
