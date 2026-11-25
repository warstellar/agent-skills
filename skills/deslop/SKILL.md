---
name: deslop
description: >
  Draft, edit, or review text for a specific audience, situation, and purpose.
  Use for product and game UI copy, including strings in code, and for
  customer-facing or published writing. Also use when asked to remove AI slop,
  fix generic prose, or tell whether wording belongs in an interface or document.
license: MIT
metadata:
  author: Ian Corvin
  version: "3.0"
---

# Deslop

Start with the reader's situation. A fluent sentence can still get in the way, explain the wrong thing, or sound as if it came from the implementation plan.

## Establish what the text needs to do

- Identify who will encounter it, where, what they already know or see, and what they need to understand, decide, do, or experience next. Use the brief, surrounding artifact, product behavior, and terminology as evidence. A product area or a component name alone is not a reader goal.
- When reviewing, compare that intended job with the job the current text actually does. Treat an audience or purpose inferred from the artifact as provisional. If the distinction changes the edit, inspect available context or give a conditional diagnosis. Ask only when the missing context prevents a sound result.
- Check fit at the scale of the problem. Look at the screen, section, or message before rewriting its lines. Supporting detail belongs where it helps the reader at that moment. An individually clear paragraph can still interrupt the task or belong somewhere else.

For interface copy, including game UI and user-visible strings in code, read [Interface copy](references/interface-copy.md). For prose patterns, worked examples, or the research behind the guidance, use [Editorial examples](references/editorial-examples.md) as needed.

## Draft, edit, or review

1. **Fix what the artifact says.** Lead with the information the reader came for. Cut or move duplicate guidance, design rationale, implementation narration, draft notes, and background the reader already has. Keep technical or contextual detail when it affects a choice, explains behavior the reader needs to understand, or enables recovery. Preserve deliberate voice and worldbuilding when they serve the experience.
2. **Keep claims true.** Preserve facts, uncertainty, scope, conditions, units, links, and user-visible terminology. Any new number, causal claim, benefit, capability, or promise needs a basis in the supplied material or verified behavior. If a needed fact is unknown, surface the gap to the requester outside the artifact. When editing, leave sound passages alone.
3. **Polish in context.** Replace vague praise, unsupported significance and attribution, staged contrasts, explanations of obvious points, and endings that merely restate the text. Use the audience's vocabulary and the register of the artifact. Read the surrounding passage for repetition and flow. Word choice, rhythm, and punctuation can point to awkward writing in context. They do not establish authorship and have no quotas.

Match the requested deliverable. A review identifies the most consequential problem with a concrete example and a practical fix. An edit or draft delivers the copy in its requested form. Keep editorial reasoning, open questions, and verification notes outside the finished copy.

This skill shares the reader-purpose check used by `diataxis-check`. For a Diátaxis review of a documentation page, that skill provides the analysis of page structure and documentation modes. A copy edit does not require classifying the document.
