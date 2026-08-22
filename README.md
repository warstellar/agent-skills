# agent-skills

[![Agent Skills](https://img.shields.io/badge/format-Agent%20Skills-b083f0)](https://agentskills.io/)

A collection of Agent Skills for Claude Code, Codex, ChatGPT, Gemini CLI, and other tools that support the open [Agent Skills](https://agentskills.io/) format.

## Install

Install everything:

```bash
npx skills add warstellar/agent-skills
```

Or pick a skill:

```bash
npx skills add warstellar/agent-skills --skill deslop
npx skills add warstellar/agent-skills --skill diataxis-check
npx skills add warstellar/agent-skills --skill decision-log
```

## Skills

### deslop

Detects, critiques, and rewrites text that sounds generically AI-written.

It catches recurring patterns in word choice, rhythm, structure, formatting, vague claims, promotional language, and other LLM habits, then rewrites toward something more specific and human.

[View skill](skills/deslop/SKILL.md)

<details>
<summary>Example</summary>

| AI version | Human version |
|---|---|
| "This isn't just a tool. It's a revolution." | "This tool cut onboarding from 3 weeks to 4 days." |
| "serves as a critical component, ensuring seamless integration" | "is the piece that connects the two systems" |

</details>

### diataxis-check

Reviews a technical-documentation page or fragment using the [Diátaxis](https://diataxis.fr/) framework.

It works from the reader's actual need, checks whether the page's scope and structure support it, and recommends one high-value structural improvement.

[View skill](skills/diataxis-check/SKILL.md)

Based on Diátaxis by Daniele Procida. See the skill's [license and attribution](skills/diataxis-check/LICENSE.md).

### decision-log

Maintains a lightweight `DECISIONS.md` log of decisions whose reasoning should survive beyond the current agent session.

It records durable changes in direction, assumptions, workflows, structure, or constraints while ignoring routine execution choices and other noise. It works across software projects, product and design work, research, knowledge bases, and other persistent agent workspaces.

[View skill](skills/decision-log/SKILL.md)

## Licensing

Unless otherwise stated in a skill's directory, this repository is licensed under the MIT License.

Some skills include their own license or attribution requirements.

See [LICENSE.md](LICENSE.md).

## Author

Ian Corvin — [github.com/warstellar](https://github.com/warstellar)