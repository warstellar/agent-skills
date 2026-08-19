---
name: diataxis-check
description: >
  Review one existing technical-documentation page or small fragment using the Diátaxis framework. Use when the user asks to check, audit, diagnose, classify, or improve documentation according to Diátaxis; identify whether content is primarily a tutorial, how-to guide, reference, or explanation; spot mixed documentation modes; or find the single most useful next Diátaxis improvement. Focus on the user need and documentation mode, not general prose quality or factual verification.
---

# Diátaxis Check

Review one documentation page or small fragment through the Diátaxis framework. Diagnose what user need the content serves, whether its mode is coherent, and the single next change that would improve the fit.

Keep the review narrow. Do not turn it into a general documentation audit or a full rewrite.

## Core model

Classify by the user's need, not by surface format, headings, or apparent difficulty.

Use the Diátaxis compass:

| Content primarily... | User is primarily... | Mode |
| --- | --- | --- |
| guiding action | acquiring skill / studying | Tutorial |
| guiding action | applying skill / working | How-to guide |
| providing knowledge | applying skill / working | Reference |
| providing knowledge | acquiring understanding / studying | Explanation |

Ask two questions:

1. Is the user trying to **act** or to **understand/know**?
2. Are they **acquiring** skill or **applying** skill they already have?

Use those answers to identify the dominant mode.

## Mode criteria

### Tutorial

Treat content as a tutorial when its main job is to provide a successful learning experience through guided action.

Look for:
- a learner who is acquiring competence;
- a deliberately managed path rather than an open-ended real-world task;
- concrete actions with visible, expected results;
- enough guidance that a novice can stay oriented and successful;
- minimal explanation and few or no optional branches.

Do not classify something as a tutorial merely because it is basic. Advanced material can still be a tutorial if the user is studying rather than working.

### How-to guide

Treat content as a how-to guide when its main job is to help an already-competent user accomplish a real-world goal or solve a problem.

Look for:
- a specific practical goal;
- directions that serve the user's work rather than teach the tool;
- instructions focused on action, with explanation kept out of the way;
- room for conditions, judgement, branches, or alternate paths when reality requires them;
- omission of background or exhaustive reference material that is not needed to complete the task.

Do not classify something as a how-to merely because it contains numbered steps. Ask whether those steps serve a real user goal or a learning experience.

### Reference

Treat content as reference when its main job is to provide authoritative technical information that users consult while working.

Look for:
- neutral description of the product, system, API, command, object, option, or behavior;
- facts, lists, tables, parameters, constraints, warnings, and compact examples;
- consistent patterns that make information easy to locate;
- structure that reflects the thing being documented where appropriate;
- little or no instruction, argument, teaching, or discursive explanation.

Examples can illustrate reference material without turning it into a how-to guide.

### Explanation

Treat content as explanation when its main job is to deepen understanding of a topic.

Look for:
- context, reasons, background, relationships, implications, or mental models;
- discussion of why something works or why a choice was made;
- comparison of alternatives or legitimate perspectives;
- a topic that can be considered away from an immediate task;
- discursive treatment rather than step-by-step instruction or neutral lookup information.

Keep explanation bounded. If it starts giving procedural directions or cataloguing product facts, those parts may belong elsewhere.

## Review workflow

Follow this sequence internally.

1. **Identify the likely user need.** Determine what the reader appears to be trying to accomplish, learn, look up, or understand. Infer from the supplied page when necessary; mark uncertainty instead of inventing context.

2. **Apply the compass.** Decide action vs cognition, then acquisition vs application.

3. **Determine the dominant mode.** Use Tutorial, How-to guide, Reference, or Explanation. Use Mixed/unclear only when the page genuinely serves competing Diátaxis needs or no coherent dominant need can be supported.

   Do not classify a page as mixed merely because it contains multiple roles, audiences, goals, interfaces, or workflows. Those can all exist within the same Diátaxis mode.

4. **Check the page against that mode.** Look at its wording, structure, assumptions about the reader, and the kinds of material it includes.

5. **Diagnose the most important problem.** Distinguish between:
   - a **mode conflict**, where some material serves a different Diátaxis user need;
   - a **scope, audience, or task-boundary problem**, where the material remains in the same mode but combines things that would serve users better separately;
   - another documentation issue that Diátaxis helps expose but does not itself classify.

   Do not force every problem into a Diátaxis category.

6. **Choose one next improvement.** Recommend the smallest change with the highest immediate value: remove, move, shorten, split, relabel, clarify, or add something specific.

If the user explicitly asks you to apply the fix, make only that focused change unless they ask for a broader rewrite.

## Guardrails

- Do not force documentation into four top-level sections. Diátaxis modes describe user needs and forms of content, not a mandatory site navigation template.
- Do not assume a page must be perfectly pure. Small amounts of another mode can support the dominant mode when they do not interrupt the user's purpose.
- Multiple audiences, roles, goals, interfaces, or workflows do not by themselves make a document mixed-mode.
- Do not call something a mode conflict unless the conflicting material actually serves a different Diátaxis user need.
- Do not force ordinary scope, audience, information-architecture, or task-boundary problems into Diátaxis terminology. Name the problem plainly when that is more accurate.
- Do not confuse tutorial vs how-to with beginner vs advanced. The distinction is study vs work.
- Do not confuse reference vs explanation with short vs long. The distinction is lookup for work vs understanding through study or reflection.
- Do not surface the Diátaxis classification just because you performed one internally. Mention the mode when it helps explain the problem or when the user asks for classification.
- Do not grade the document numerically. Avoid invented scores such as "7/10 Diátaxis compliance."
- Do not claim to verify factual accuracy, completeness, technical correctness, accessibility, SEO, grammar, or general style unless the user separately asks for those checks and provides enough evidence.
- Do not turn the review into a comprehensive redesign. Prefer one meaningful improvement over a backlog of marginal suggestions.
- If several pages are supplied, review one at a time unless the user explicitly asks for a batch or information-architecture review.

## Output

Write the review as concise, natural editorial feedback, not as a diagnostic form.

Lead with the main observation about how well the page serves the reader's need. Explain the most important problem using concrete evidence from the page, then recommend one practical next improvement.

Use Diátaxis terminology when it genuinely helps explain the issue. Do not force the response into fixed fields such as "Dominant mode", "User need", "Mode conflict", or confidence levels.

If the main problem is not a Diátaxis mode conflict, say what it actually is: for example, mixed audiences, several tasks on one page, misplaced background material, or unclear scope.

If the page already fits its purpose well, say so instead of inventing a problem.

If the user explicitly asks for classification, a formal audit, or the reasoning through the Diátaxis compass, provide a more structured diagnosis.

Keep the answer proportional to the source. Quote or point to short passages when that makes the feedback easier to verify.

## Example

Input excerpt:

> # Download a topic as PDF
>
> First, an administrator must enable single-topic PDF downloads under **Settings > Branding > Reader Interface**.
>
> Contributors can then open a topic in the editor and select **Download as PDF**.
>
> Readers can also download the topic from the Reader UI using the PDF button.

Review:

This is essentially a how-to, but the bigger problem is not a Diátaxis mode conflict. The page combines setup work for an administrator with the actual download task for Contributors and Readers.

Someone who arrives because they want to download a topic is forced through configuration steps they may not have permission to perform. The setup and the user action are both goal-oriented instructions, but they serve different people at different moments.

I would split them into two how-to pages: one for configuring single-topic PDF downloads, and one for downloading a topic as PDF. The second page only needs a short note linking to the configuration instructions if the download option is unavailable.