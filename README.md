# agent-skills

A collection of [Agent Skills](https://code.claude.com/docs/en/skills) for Claude Code and other coding agents.

## Install

```bash
npx skills add warstellar/agent-skills
```

Or install a single skill directly by pointing at its folder — check the CLI's docs for the exact syntax (`npx skills --help`).

## Skills

- **[deslop](skills/deslop/SKILL.md)** — detects, critiques, and rewrites text to remove AI writing patterns (word choice, rhythm, structural tells) so it reads like a specific, thoughtful human wrote it.

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
