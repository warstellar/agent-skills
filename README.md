# agent-skills

[![Agent Skills](https://img.shields.io/badge/format-Agent%20Skills-b083f0)](https://agentskills.io/)

A collection of Agent Skills for Claude Code, Codex, ChatGPT, Gemini CLI, and other tools that support the open Agent Skills format.

## Install

Install all skills from this repository:

```bash
npx skills add warstellar/agent-skills
```

Or install a single skill:

```bash
npx skills add warstellar/agent-skills --skill deslop
```

```bash
npx skills add warstellar/agent-skills --skill diataxis-check
```

Check the CLI docs for the full syntax:

```bash
npx skills --help
```

## Skills

### deslop

Detects, critiques, and rewrites text to remove common AI-writing patterns so it reads like a specific, thoughtful human wrote it.

It looks at word choice, rhythm, structure, formatting, vague claims, promotional language, and other recurring LLM writing habits.

[View skill](skills/deslop/SKILL.md)

<details>
<summary>Example</summary>

| AI version | Human version |
|---|---|
| "This isn't just a tool. It's a revolution." | "This tool cut onboarding from 3 weeks to 4 days." |
| "serves as a critical component, ensuring seamless integration" | "is the piece that connects the two systems" |

</details>

### diataxis-check

Reviews one technical-documentation page or fragment using the [Diátaxis](https://diataxis.fr/) framework.

It identifies the user need and dominant documentation mode, spots meaningful mixing between tutorials, how-to guides, reference, and explanation, and recommends one concrete next improvement.

[View skill](skills/diataxis-check/SKILL.md)

Based on Diátaxis by Daniele Procida. See the skill's [license and attribution](skills/diataxis-check/LICENSE.md).

## Repository structure

Each skill lives in its own directory:

```text
skills/
  <skill-name>/
    SKILL.md
```

A skill may also include supporting files when needed:

```text
skills/
  <skill-name>/
    SKILL.md
    agents/
    references/
    scripts/
    assets/
    LICENSE.md
```

`SKILL.md` contains the skill's name, description, and instructions. The other files are optional and depend on what the skill needs.

## Adding a skill

Create a directory under `skills/` and add a `SKILL.md` with YAML frontmatter:

```yaml
---
name: example-skill
description: Describe what the skill does and when an agent should use it.
---
```

Keep skills self-contained where practical. Add references, scripts, or other files only when they materially improve the skill.

## Licensing

Unless otherwise stated in a skill's directory, the contents of this repository are licensed under the MIT License.

Some skills are based on or adapted from third-party work and use different licenses. When a skill contains its own `LICENSE` or `LICENSE.md`, that license applies to the skill instead of the repository default.

See [LICENSE.md](LICENSE.md).

## Author

Ian Corvin — [github.com/warstellar](https://github.com/warstellar)