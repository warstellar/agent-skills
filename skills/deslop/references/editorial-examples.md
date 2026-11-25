# Editorial examples

Use these examples to diagnose a writing problem in context. Match the source language, reader's register, and existing voice. Judge the result by what the reader gains.

| Problem | Example and edit |
| --- | --- |
| The draft contains the writing brief | A release note that says «Мы вынесли действие в меню, чтобы не перегружать экран» leads with a design decision. If users need to find the moved control, write «Команда „Экспорт“ теперь в меню „Отчёт“», provided those labels and placement are verified. A design handoff may need the rationale. |
| The line delivers emphasis instead of information | “The update marks a major milestone in collaboration.” State the change, such as a new shared review action, when the source confirms it. Omit the milestone claim if there is no evidence for it. |
| The draft makes a promise out of a mechanism | “Failed requests retry twice, ensuring users never lose work.” Keep the retry behavior if confirmed, including which failures trigger a retry. A retry count alone cannot establish the outcome. |
| A simplification loses an important qualifier | “If volume stays below 5,000 events per day, we expect the current plan to cover it.” Keep the threshold and the uncertainty. “The current plan covers it” turns an estimate into a promise. |
| A style change makes terms less precise | In a reference for developers, keep terms such as “idempotency key” when that is what the reader needs to look up. Preserve syntax, defaults, and exact labels. Simplify the surrounding sentence if it is hard to follow. |
| A rhetorical contrast carries no distinction | “It’s not just a dashboard. It’s a new way to work.” Ask what someone can do there that they could not do before. “The filter changes the current view. It does not change the saved report” explains a meaningful behavior difference. |
| Repetition masquerades as structure | If a heading, a bold lead, and a final one-line takeaway make the same point, keep the form that serves scanning or reading in that location. Repeat an exact control name where the reader needs to recognize it. |
| A handoff turns into an account of the agent's work | “Updated the flow while preserving the existing architecture and avoiding regressions” answers little by itself. Report the changed behavior, evidence, or pending decision the recipient needs. Mention the architecture when it is relevant to their work. |

For release notes, use the change and its practical effect for the reader. Preserve limitations and any migration or action that matters. For technical instructions, keep steps, prerequisites, and expected results where they are needed. In customer messages, use shared context and lead with the decision, answer, or request. In a social post or opinion piece, preserve the author's actual stance, uncertainty, and cadence. A genuine aside can do more work than several polished transitions.

## Where the guidance comes from

- [Diátaxis](https://diataxis.fr/compass/) and the local `diataxis-check` skill informed the check for the difference between what an artifact appears to do and what the reader needs in that situation.
- [Wikipedia's Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) is an evolving guide to Wikipedia edits. Its edit-summary examples illustrate process text leaking into an artifact. Its historical section is a reason to retire fixed detection rules from earlier versions of this skill.
- The [EMNLP 2026 study of style across genres and models](https://aclanthology.org/2026.findings-emnlp.1375/) and [El Attar et al.'s English-language preprint](https://arxiv.org/abs/2606.04177) found that many stylistic measures depend on the genre, domain, or model. These are corpus-level findings. They do not supply a rule for judging a Russian tooltip or an individual author's voice.
