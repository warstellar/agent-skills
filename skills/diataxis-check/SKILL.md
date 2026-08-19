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

Follow this sequence.

1. **Identify the likely user need.** State what the reader appears to be trying to accomplish, learn, look up, or understand. Infer from the supplied page when necessary; mark uncertainty instead of inventing context.
2. **Apply the compass.** Decide action vs cognition, then acquisition vs application.
3. **Name the dominant mode.** Use Tutorial, How-to guide, Reference, Explanation, or Mixed/unclear when no coherent dominant need can be supported.
4. **Check the page against that mode.** Look for evidence in wording, structure, assumptions about the reader, and the kind of material included.
5. **Find meaningful mode conflicts.** Identify only passages that pull the reader toward a different user need. Do not flag every sentence that resembles another mode.
6. **Choose one next improvement.** Recommend the smallest change with the highest immediate value: remove, move, shorten, split, relabel, or add something specific.

If the user explicitly asks you to apply the fix, make only that focused change unless they explicitly ask for a broader rewrite.

## Guardrails

- Do not force documentation into four top-level sections. Diátaxis modes describe user needs and forms of content, not a mandatory site navigation template.
- Do not assume a page must be perfectly pure. Small amounts of another mode can support the dominant mode when they do not interrupt the user's purpose.
- Do not confuse tutorial vs how-to with beginner vs advanced. The distinction is study vs work.
- Do not confuse reference vs explanation with short vs long. The distinction is lookup for work vs understanding through study/reflection.
- Do not grade the document numerically. Avoid invented scores such as "7/10 Diátaxis compliance."
- Do not claim to verify factual accuracy, completeness, technical correctness, accessibility, SEO, grammar, or style unless the user separately asks for those checks and provides enough evidence.
- Do not turn the review into a comprehensive redesign. Prefer one concrete improvement over a backlog of marginal suggestions.
- If several pages are supplied, review one at a time unless the user explicitly asks for a batch or information-architecture review.

## Output

Default to a compact diagnostic:

**Dominant mode:** <Tutorial | How-to guide | Reference | Explanation | Mixed/unclear> — <high/medium/low confidence>

**User need:** <one sentence describing the need this page appears to serve>

**Why:** <2-4 concise observations grounded in the supplied content>

**Mode conflict:** <the most important conflicting passage or "No meaningful conflict found">

**Next improvement:** <one specific, actionable change>

Keep the answer proportional to the source. Quote or point to short passages when that makes the diagnosis easier to verify.

## Example

Input excerpt:

> # How to configure session timeout
> 1. Open **Security > Sessions**.
> 2. Set **Idle timeout** to 30 minutes.
>
> The session service stores state in Redis. This architecture was chosen to support horizontal scaling and simplify failover across application nodes. Earlier versions stored session state in process memory, which created several operational limitations.
>
> 3. Select **Save**.

Review:

**Dominant mode:** How-to guide — high confidence

**User need:** Configure the idle session timeout while already administering the product.

**Why:** The page is organized around a specific operational goal and gives executable directions to achieve it. It assumes the reader can navigate the product without being taught the basics.

**Mode conflict:** The Redis/history paragraph switches from guiding work to explaining architecture and design rationale. That is explanation material and interrupts the action sequence.

**Next improvement:** Move the architecture paragraph to an explanation page and replace it here with a short link for readers who want the background.

## Framework basis

Apply the Diátaxis framework as a pragmatic diagnostic tool. Its four modes are tutorial, how-to guide, reference, and explanation, distinguished by whether the user needs action or cognition and whether they are acquiring or applying skill. Use the framework to improve fit to user needs; do not present it as a complete test of documentation quality.