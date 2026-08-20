---
name: diataxis-check
description: >
  Review one existing technical-documentation page or small fragment using
  Diátaxis as a content-design framework. Use when the user asks whether a
  documentation page is well structured, logically scoped, organized around
  the intended reader's need, or appropriate for its audience; asks to audit
  or improve a page according to Diátaxis; or wants to understand what is wrong
  with a documentation topic and how to improve it. Infer the intended reader
  and their need, use Diátaxis to establish the expected documentation mode,
  consult the relevant mode-specific diagnostic guidance, diagnose page-level
  content architecture, and recommend one high-value improvement. Do not treat
  Diátaxis classification itself as the goal or claim general documentation
  quality.
---

# Diátaxis Check

Review one existing documentation page or small fragment.

The goal is to determine whether the page is coherently designed around the
need of its intended reader, and whether its scope, structure, and content make
sense for that need.

Use Diátaxis as the reasoning framework. Tutorial, how-to, reference, and
explanation are models that establish what the page should do for its reader.
Classification is an intermediate step, not the primary output.

Focus on page-level content architecture and logic rather than prose quality,
factual verification, or comprehensive documentation redesign.

## Terminology

Keep these roles distinct:

- **Requester** — the person asking for the documentation review.
- **Reader** or **intended reader** — the person the documentation itself is
  meant to serve.

When reasoning about needs, goals, work, competence, or audience, refer to the
documentation reader, not the requester.

## Core model

Start with the intended reader's situation, not the document's apparent format.

Diátaxis distinguishes documentation along two dimensions:

| Reader need | Acquiring skill or understanding | Applying skill or knowledge |
| --- | --- | --- |
| **Action** | Tutorial | How-to guide |
| **Cognition** | Explanation | Reference |

Ask:

1. Does the intended reader primarily need to **do something**, or to **know or
   understand something**?
2. Are they **acquiring** new competence or understanding, or **applying**
   existing competence while working?

Use the answer to infer what kind of documentation would best serve that
reader.

Then use the relevant mode as a model for what the page's content architecture
should accomplish.

## Mode references

After inferring the likely mode, read the corresponding diagnostic model before
evaluating the page in detail:

- **Tutorial** — [references/tutorial.md](references/tutorial.md)
- **How-to guide** — [references/how-to.md](references/how-to.md)
- **Reference** — [references/reference.md](references/reference.md)
- **Explanation** — [references/explanation.md](references/explanation.md)

Read the reference for the expected dominant mode, not all four by default.

If the page genuinely appears to serve two competing reader needs and that
distinction matters to the diagnosis, read the relevant second reference as
well.

If the intended need itself remains ambiguous between two modes, read both
plausible references and use them to clarify the distinction.

Use the references to derive concrete expectations for purpose, scope,
structure, flow, boundaries, and supporting content.

Do not use them merely to prove that another Diátaxis mode is present.

## Review workflow

Follow this reasoning internally.

### 1. Infer the intended reader and their need

Determine why someone would reasonably open this page.

Look at:

- the title;
- the introduction;
- headings and section boundaries;
- actions the page asks someone to perform;
- assumptions about knowledge or competence;
- roles and permissions;
- the outcome or understanding the page appears to promise.

Try to express the reader's need plainly, for example:

- configure session timeout;
- understand why deployments behave this way;
- look up the parameters of an endpoint;
- learn to create a first project.

Do not confuse a product feature with a reader need.

"Visual Workflow Editor" describes a thing.
"Change a workflow and apply it to the portal" describes something a reader
might need to accomplish.

If several roles appear, ask whether they share one coherent need or represent
different jobs.

If the page appears to serve several substantially different needs, preserve
that ambiguity. Do not invent a single purpose merely to make classification
easier.

### 2. Use Diátaxis to establish the expected mode

Apply the action/cognition and acquisition/application dimensions.

Determine which mode would best serve the inferred reader need:

- Tutorial
- How-to guide
- Reference
- Explanation

Use the classification to establish an expectation about the document, not
merely to attach a label to it.

### 3. Load the diagnostic model

Read the corresponding mode reference.

Use it to determine what follows from this reader situation:

- what should organize the page;
- what belongs inside its scope;
- what kind of sequence or structure makes sense;
- what assumptions about the reader are appropriate;
- what supporting material is useful;
- what common structural failures to look for.

Do not read every mode reference for completeness.

### 4. Compare the actual page with the expected model

Evaluate the actual content architecture against the expectations derived from
the reader's need and the relevant mode reference.

Do not ask merely whether the page "looks like" a tutorial, how-to, reference,
or explanation.

Ask whether it serves the reader in the way that this kind of documentation
should.

Look for structural problems such as:

- **Unclear purpose** — there is no clear reader need around which the page is
  organized.
- **Scope that is too broad** — several independently useful tasks or subjects
  have been bundled together without a strong reader-centered reason.
- **Task-boundary problems** — setup, administration, execution, maintenance,
  troubleshooting, or other distinct jobs are combined in a way that weakens
  the reader's path.
- **Audience or role mismatch** — different sections assume substantially
  different permissions, competence, responsibilities, or goals.
- **Structural mismatch** — the organization follows the wrong logic for how
  the reader needs to work, learn, look information up, or build understanding.
- **Mode mismatch** — the page's form does not fit the reader need it appears
  intended to serve.
- **Mode conflict** — material serving another Diátaxis need substantially
  interrupts or competes with the dominant reader need.
- **Poor placement of supporting material** — useful prerequisites, facts,
  explanations, warnings, examples, or alternatives appear where they disrupt
  rather than support the page's purpose.

These are diagnostic possibilities, not boxes that must all be checked.

A page can be structurally weak without containing a Diátaxis mode conflict.

### 5. Judge the page as a coherent unit

Consider why this material belongs together.

Ask:

- Is there a clear reason for this page to exist?
- Would the intended reader recognize that reason?
- Does the page mostly serve that need?
- Does its scope make sense for that need?
- Does the grouping of information support the reader's situation?
- Does the sequence follow the logic appropriate to this mode?
- Are different tasks, roles, topics, or modes combined because the reader
  benefits from having them together?
- Or are they grouped merely because they concern the same product, feature,
  interface, or technical area?

Do not equate "about the same feature" with "belongs on the same page."

Conversely, do not split material simply because several roles, interfaces,
sub-actions, or modes are present. Keep them together when they form a coherent
experience for the reader.

### 6. Find the highest-value problem

Identify the structural problem that most weakens the page's ability to serve
its intended reader.

Prefer a root problem over its symptoms.

For example, several awkward sections may all follow from one deeper problem:
the page is organized around product features instead of the reader's task.

Do not produce a backlog of every possible improvement.

If the page already has a coherent purpose and architecture for its reader,
say so rather than inventing a problem.

### 7. Recommend one next improvement

Recommend the smallest practical change that would meaningfully improve the
page.

Depending on the diagnosis, this might mean:

- clarify or narrow the reader need;
- split an independent task into another page;
- reorganize sections around the reader's workflow;
- move one-time setup out of a recurring task;
- separate material intended for substantially different roles;
- turn a feature-oriented collection into task-oriented guidance;
- restructure reference material for predictable lookup;
- move substantial explanation out of an action-oriented flow;
- bound an explanation around a clearer conceptual question;
- remove or relocate material that does not serve the page's purpose.

Explain why the change follows from the intended reader's need.

If the requester asks to apply the recommendation, make only that focused
change unless they explicitly request a broader rewrite.

## Supporting content and mode boundaries

Documentation does not need to be perfectly mode-pure.

A how-to can contain field definitions, constraints, expected results, or short
explanations. A tutorial can contain reference facts. Reference can include
examples. Explanation can mention practical consequences.

Treat cross-mode material as a problem only when it meaningfully interferes
with the dominant reader need.

The presence of another Diátaxis mode is evidence to inspect, not automatically
a reason to move or split content.

Use the relevant mode reference to judge whether supporting material helps or
disrupts the page's purpose.

## Guardrails

- Evaluate one page or small fragment at a time unless the requester explicitly
  asks for a broader information-architecture review.
- If only a fragment is provided, do not make unsupported claims about the
  architecture of the unseen page.
- Do not force documentation into four top-level sections. Diátaxis describes
  reader needs and documentation forms, not a mandatory site structure.
- Do not assume every page must contain exactly one action, role, interface, or
  technical component.
- Do not call multiple roles, tasks, or interfaces a Diátaxis mode conflict
  unless they genuinely represent competing reader needs.
- Do not confuse tutorial vs how-to with beginner vs advanced. The distinction
  is learning versus performing real work.
- Do not confuse reference vs explanation with short versus long. The
  distinction is consultation during work versus developing understanding.
- Do not treat classification as the outcome of the review. Use it to reason
  about what the page should do.
- Read only the mode references needed for the current diagnosis.
- Do not recommend splitting material merely to achieve mode purity.
- Do not grade Diátaxis compliance numerically.
- Do not claim to verify factual accuracy, technical correctness,
  completeness, accessibility, SEO, grammar, or prose style unless the
  requester separately asks for those checks and provides enough evidence.
- Do not turn a page review into a comprehensive documentation redesign.
- Do not invent problems when the page already serves its intended reader well.

## Output

Write concise, natural editorial feedback rather than a diagnostic form.

Start with the main conclusion about the page: what it appears to help its
intended reader do or understand, and whether the page is coherently built
around that need.

Explain the most important structural problem using concrete evidence from the
page.

Then recommend one practical next improvement and explain why it would better
serve the intended reader.

Use Diátaxis terminology when it genuinely clarifies the diagnosis, but do not
force the response into fixed fields such as:

- Dominant mode
- User need
- Mode conflict
- Confidence

Do not narrate the internal process of loading references or applying the
compass unless the requester asks for that reasoning.

The feedback should describe the actual documentation problem, not celebrate
the detection of a Diátaxis violation.

If the requester explicitly asks for classification, a formal Diátaxis audit,
or an explanation of the reasoning, provide the underlying mode and compass
analysis.