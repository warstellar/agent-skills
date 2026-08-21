---
name: diataxis-check
description: >
  Review one existing technical-documentation page or small fragment using
  Diátaxis as a content-design framework. Use when the user asks whether a
  documentation page is well structured, logically scoped, organized around
  the intended reader's need, appropriate for its audience, or how it could be
  improved according to Diátaxis. Establish the intended reader and desired
  outcome from requester-provided context when available; otherwise infer them
  from the page as hypotheses rather than ground truth. Compare the page's
  apparent purpose with its intended purpose before applying the Diátaxis
  compass and mode-specific diagnostic guidance. Identify the most important
  page-level problem and recommend one focused improvement. Classification is
  an intermediate reasoning step, not the goal of the review.
---

# Diátaxis Check

Review one existing documentation page or small fragment.

The goal is to determine:

- what the page appears to help its intended reader do or understand;
- what kind of documentation would best serve that need;
- whether the page's scope, structure, and content support that purpose;
- what single change would improve it most.

Use Diátaxis as a reasoning framework, not as a compliance checklist.

## Terminology

Keep these roles distinct:

- **Requester** — the person asking for the review.
- **Reader** or **intended reader** — the person the documentation itself is
  meant to serve.

When reasoning about needs, competence, work, study, goals, or understanding,
refer to the documentation reader, not the requester.

## Scope

By default, review one page or a small supplied fragment.

Focus on page-level content design:

- purpose;
- reader need;
- scope;
- grouping;
- sequence or organization;
- fit between the reader need and the documentation form;
- placement of supporting material;
- interruptions to the reader's current purpose.

Do not automatically expand the review into a site-wide information
architecture analysis.

If only a fragment is supplied, make claims only about that fragment unless
the surrounding page is visible.

## Establish the reader situation

Do not treat the page as authoritative evidence of its own intended purpose.

Keep two things distinct:

- **Intended reader and outcome** — who the documentation is supposed to serve
  and what it is supposed to help them accomplish or understand.
- **Apparent reader and outcome** — who the page itself appears to serve and
  what it appears to help them accomplish or understand.

Use evidence in this order:

1. requester-provided context about the intended audience, goal, workflow, or
   desired outcome;
2. other explicit context supplied with the page;
3. evidence from the page itself.

When the requester provides an intended reader or outcome, treat that context
as the evaluation target. Do not silently replace it with a different purpose
inferred from the page.

When the intended reader or outcome is not known, infer the apparent reader
situation from the page, but treat that inference as a hypothesis rather than
ground truth.

If materially different plausible purposes would lead to different review
results, ask the requester for the missing context before giving an overall
positive or negative judgement.

A coherent page can still be the wrong page for its intended purpose.

The reader need is situational.

An experienced practitioner can be studying something unfamiliar. A beginner
can be performing real work. Do not equate tutorial with beginner or how-to
with advanced.

Try to state the need in reader terms.

Prefer:

- configure session timeout;
- rotate an API key;
- understand why deployments are immutable;
- look up the parameters of an endpoint;
- learn to create and deploy a first project.

Avoid treating a product object as a reader need.

For example:

> Visual Workflow Editor

names a product object.

> Change a workflow and apply it to the portal

describes a reader goal.

## Use the Diátaxis compass

Classify the reader situation along two dimensions:

| | Acquisition / study | Application / work |
| --- | --- | --- |
| **Action / doing** | Tutorial | How-to guide |
| **Cognition / knowing** | Explanation | Reference |

Ask both questions:

1. Does the reader primarily need **action** or **cognition**?
2. Is the reader **acquiring** skill or knowledge, or **applying** existing
   skill or knowledge?

Use the terms as practical distinctions:

- **Action** — practical steps, doing, knowing how.
- **Cognition** — theoretical or propositional knowledge, knowing that,
  thinking.
- **Acquisition** — study.
- **Application** — work.

Do not decide from one axis alone.

For example:

- both tutorials and how-to guides concern action;
- both how-to guides and reference serve work;
- both reference and explanation concern cognition;
- both tutorials and explanation serve study.

The second axis is often what resolves an apparent similarity.

## Apply the compass to both need and content

Use the compass in two separate ways.

First, determine what the **reader needs**.

Then inspect what the **page actually does**.

Do not assume that authorial intent, navigation placement, title, and actual
content necessarily agree.

A page can be called a tutorial while functioning as task guidance. A page
placed under reference can contain a substantial conceptual discussion.

The mismatch between the reader situation and the actual content is often more
useful than the label itself.

## Use the compass at the necessary scale

Establish the page's primary job at whole-page level.

When a particular section or passage appears to interfere with that job, apply
the same distinctions locally.

A page can contain local material that serves another Diátaxis need.

Do not treat that fact alone as a defect.

Ask whether the local material supports the page's primary job or creates a
substantial competing need.

## Load the relevant mode guidance

After inferring the reader situation, read the corresponding diagnostic
reference:

- Tutorial — [references/tutorial.md](references/tutorial.md)
- How-to guide — [references/how-to.md](references/how-to.md)
- Reference — [references/reference.md](references/reference.md)
- Explanation — [references/explanation.md](references/explanation.md)

Read the expected dominant mode's reference before evaluating the page in
detail.

Do not read all four by default.

Read a second reference when:

- the reader need remains genuinely ambiguous between two modes;
- the page substantially serves two competing needs;
- a neighboring-mode distinction is necessary to diagnose the problem.

Use the reference to establish concrete expectations for the page's purpose,
scope, organization, reader assumptions, and boundaries.

## Review workflow

### 1. Establish the evaluation target

Keep the document's **intended purpose** separate from its **apparent purpose**.

The intended purpose is the external reason this document is supposed to
exist: who it is meant to serve, in what situation, and what outcome it is
supposed to produce.

The apparent purpose is what the document itself appears or claims to help the
reader do or understand.

Never establish the intended purpose from the document under review itself.

Statements in the page title, introduction, headings, navigation, or body about
who the page is for or what it will accomplish are evidence of the page's
apparent purpose only. They are not independent evidence that this is the
correct purpose for the page.

Establish the intended purpose only from requester-provided or other external
context.

If external context provides an intended reader or outcome, use it as the
evaluation target and compare the page's apparent purpose against it.

If no external intended purpose is available, do not infer one. Continue by
evaluating the page against its apparent purpose, but explicitly limit the
conclusion to internal coherence. Do not conclude that the page is appropriate
for its real documentation or product goal.

Then inspect the page to determine its apparent reader and outcome using:

- title and introduction;
- headings;
- actions the reader is asked to perform;
- information the reader is expected to consult;
- questions the page appears to answer;
- assumptions about existing competence;
- expected outcome or understanding.

For action-oriented documentation, state the apparent outcome as a concrete
end state: what has the reader accomplished, produced, configured, or become
able to do by the end?

For cognition-oriented documentation, state what the reader should understand
or be able to reason about by the end.

If several substantial apparent reader needs are present, preserve that finding
rather than inventing one artificial purpose.

### 2. Determine the expected mode

Apply both compass dimensions to the reader situation.

Use the result to establish what kind of documentation should serve that need.

Classification is a hypothesis about the page's obligations, not the review
result.

### 3. Read the relevant diagnostic model

Load the corresponding reference.

Use it to establish what should determine:

- the page's scope;
- the page's structure;
- the reader assumptions;
- the type of progression or organization;
- appropriate supporting material;
- likely neighboring-mode failures.

### 4. Check purpose fit before mode fit

If an externally established intended purpose is available, first compare it
with the page's apparent purpose.

A mismatch between intended and apparent purpose takes precedence over
Diátaxis mode quality.

A document can be an excellent tutorial, how-to guide, reference page, or
explanation and still be the wrong document for the intended reader outcome.

If no external intended purpose is available, do not make a positive judgement
about purpose fit. Evaluate only whether the page is internally coherent
relative to the purpose it appears to pursue.

Then ask whether the page serves the intended reader need, when known, in the
way that the expected mode requires.

For action-oriented documentation, state the concrete end state and check
whether each major section advances the reader toward that same end state.

Do not mistake a sequence of individually valid actions for a coherent journey.
Several feature demonstrations, tasks, or visible results do not form one
tutorial or how-to merely because they can be performed in sequence.

Look for concrete problems such as:

- the page's apparent purpose differs from its intended purpose;
- the page has no stable reader need;
- its major sections do not advance one coherent reader outcome;
- its scope follows a product or topic boundary that does not fit the reader
  situation;
- several independently meaningful tasks or subjects are bundled together;
- the organization follows the wrong logic for learning, working, consulting
  information, or building understanding;
- the page assumes substantially different levels of competence in different
  sections;
- a supporting passage creates a substantial competing reader need;
- material appears substantially before or after the point where the reader
  needs it;
- the page requires avoidable switching, backtracking, or interruption of the
  reader's current purpose.

Do not force every problem into the category of "mode mixing."

A page can be structurally weak while remaining entirely within one Diátaxis
mode.

### 5. Check why the material belongs together

Ask why the page's major sections form one page.

A shared product feature, interface, object, or technical area is not by
itself sufficient reason.

Check whether the grouping follows from the relevant reader need and mode.

Conversely, do not split a page merely because it contains:

- several actions;
- several interfaces;
- several examples;
- several roles;
- local material from another mode.

The question is whether those elements form one coherent experience for the
intended reader.

### 6. Distinguish support from interference

Material from another mode can be useful support.

Examples:

- concise parameter information inside a how-to;
- a short reason inside a tutorial;
- a usage example inside reference;
- factual examples inside explanation.

Treat such material as a problem only when it substantially changes or
interrupts what the reader is there to do.

Typical signs include:

- the reader must stop performing work and begin studying a separate subject;
- lookup information is obscured by discussion;
- a learner must process an extended conceptual digression before continuing;
- an explanation turns into a complete practical procedure;
- a supporting passage grows into an independently useful document.

Do not recommend moving material solely to achieve mode purity.

### 7. Identify the highest-value problem

Prefer a root problem that explains several symptoms.

For example:

- repeated awkward sections may follow from organizing a how-to around product
  features instead of a human project;
- missing expected results may reveal that a tutorial is being treated as a
  procedure rather than a managed learning experience;
- difficult lookup may follow from reference being written as continuous
  explanatory prose.

Do not produce a backlog of every possible improvement.

If the page serves the known intended reader and outcome coherently, say so.

If the intended purpose is only inferred from the page itself, phrase any
positive judgement conditionally. Do not use the page's internal coherence as
evidence that the inferred purpose is the correct purpose.

### 8. Recommend one next improvement

Recommend one next change that addresses the highest-value problem you identified.

Match the level of the recommendation to the level of the problem. Do not
reduce a structural or purpose-level problem to a cosmetic or local edit merely
to keep the recommendation small.

The recommendation should still be bounded enough to act on without requiring
a complete redesign of the documentation.

Explain why this change follows from the reader situation and the diagnosed
problem.

Do not produce a complete replacement or redesign unless the requester asks
for one.

## Treat friction as evidence, not proof

If a page is unusually difficult to classify or organize, or if supposedly
appropriate material repeatedly feels hard to place, reconsider the reader
need and expected mode.

Do not use intuition alone to override the compass.

At the same time, do not manufacture a mode conflict merely because a passage
looks superficially different.

Use the reader situation to resolve the ambiguity.

## Diátaxis is not a required top-level structure

Do not require documentation to contain four top-level sections named
Tutorials, How-to, Reference, and Explanation.

Do not recommend creating empty mode sections merely to reproduce the map.

Diátaxis can be applied locally to existing documentation.

For this skill, improve the material in front of you rather than designing an
ideal complete documentation system.

## Quality limits

Diátaxis does not verify functional qualities such as:

- factual accuracy;
- technical correctness;
- completeness;
- consistency with the product;
- precision.

It also does not replace accessibility, SEO, visual design, UX, or other
specialist review.

Applying Diátaxis can expose signs of functional-quality problems.

For example, a reference structure may reveal an apparent coverage gap, or
removing explanation from a tutorial may reveal that the learner was expected
to infer a missing step.

Treat such findings as evidence of a possible problem, not as verification.

This skill can judge fit to reader needs, mode-specific content design, and
reader flow. These require judgement rather than numerical measurement.

Do not assign a Diátaxis compliance score or percentage.

Do not claim that correct use of Diátaxis proves general documentation
quality.

## Output

Write concise, natural editorial feedback.

When an externally established intended reader or outcome is available, start
with that evaluation target and say whether the page is coherently designed
around it.

When no external intended purpose is available, clearly distinguish the page's
apparent purpose from an actually established intended purpose.

Do not say that a page "works well", "serves its reader well", "is appropriate
for its audience", or make an equivalent unconditional positive judgement when
the intended purpose has only been derived from the page itself.

In that case, limit the conclusion to internal coherence. For example:

> This page is internally coherent as a tutorial for X. From the page alone,
> however, I cannot determine whether X is the outcome this documentation is
> actually supposed to serve.

If missing audience or outcome context could materially change the verdict,
say what context is missing. Ask the requester for it when answering the
question responsibly requires it.

If the page's apparent purpose materially differs from an externally
established intended purpose, make that mismatch the primary finding even when
the page follows its Diátaxis mode well internally.

Then explain the most important problem using concrete evidence from the page.

Recommend one practical next improvement and explain why it would better serve
the intended reader or outcome.

Use Diátaxis terminology when it clarifies the diagnosis, but do not force the
response into fields such as:

- Dominant mode
- Reader need
- Mode conflict
- Confidence
- Compliance score

Do not describe the internal review workflow, including applying the compass,
classifying the mode, or consulting mode references, unless the requester
explicitly asks for the reasoning or a formal Diátaxis analysis.

State the result of that reasoning directly in reader-centered terms.

Instead of:

> I applied the compass and identified this as a how-to guide...

Prefer:

> This page appears to help an experienced reader modify and publish a workflow.

If the requester explicitly asks for classification, a formal Diátaxis audit,
or the underlying reasoning, provide the compass and mode analysis.