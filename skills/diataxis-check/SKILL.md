---
name: diataxis-check
description: >
  Review one existing technical-documentation page or small fragment using
  Diátaxis as a content-design framework. Use when the user asks whether a
  documentation page is well structured, logically scoped, organized around
  the right user need, or appropriate for its audience; asks to audit or
  improve a page according to Diátaxis; or wants to understand what is wrong
  with a documentation topic and how to improve it. Diagnose page-level
  content architecture and recommend the single most useful next improvement.
  Do not treat Diátaxis classification itself as the goal.
---

# Diátaxis Check

Review one existing documentation page or small fragment.

The goal is to determine whether the page is coherently organized around a
real user need and whether its content and structure make sense for that need.

Use Diátaxis as the reasoning framework. Classification into tutorial, how-to,
reference, or explanation is an intermediate step that helps determine what
the page should do. It is not the primary output.

Focus on page-level content architecture and logic rather than prose quality,
factual verification, or a comprehensive documentation redesign.

## Core model

Start with the user's situation, not the document's apparent format.

Diátaxis distinguishes documentation along two dimensions:

| User need | Acquiring skill or understanding | Applying skill or knowledge |
| --- | --- | --- |
| **Action** | Tutorial | How-to guide |
| **Cognition** | Explanation | Reference |

Ask:

1. Does the user primarily need to **do something**, or to **know or understand something**?
2. Are they **acquiring** new competence or understanding, or **applying** existing competence while working?

Use the answer to infer what kind of document would best serve the user.

Then evaluate the actual page against that expectation.

## What each mode implies

### Tutorial

A tutorial serves a learner who is acquiring competence through guided action.

Expect:

- a managed learning experience rather than a real-world task;
- a clear path controlled by the tutorial;
- concrete actions with visible results;
- enough context to keep the learner oriented;
- minimal branching and optionality;
- only the explanation and reference material needed to support the lesson.

A tutorial is not merely a beginner how-to. Its defining purpose is learning.

### How-to guide

A how-to guide serves a competent user trying to accomplish a real-world goal.

Expect:

- a recognizable user goal;
- content organized around completing that goal;
- actionable directions;
- prerequisites that are relevant to the task;
- conditions and branches when the real task requires them;
- supporting facts or explanation only where they help the user complete the work.

A how-to guide can contain several steps, interfaces, or related sub-actions.
The question is whether they form a coherent task from the user's point of view.

### Reference

Reference serves a user who needs authoritative information while working.

Expect:

- factual, technical description rather than a guided task;
- predictable lookup-oriented structure;
- terminology, parameters, fields, constraints, options, tables, lists, or examples;
- organization that reflects the product, API, system, or other machinery being described;
- consistent patterns that make information easy to find.

Reference may contain small examples or procedural hints, but its main job is
to provide information for consultation.

### Explanation

Explanation serves a user who wants to understand a subject more deeply.

Expect:

- context, reasons, relationships, implications, or mental models;
- discussion of why something works or is designed a certain way;
- alternatives, trade-offs, history, or background when relevant;
- a coherent topic that can be understood through reading and reflection.

Explanation may refer to practical work, but its main purpose is understanding,
not completing that work.

## Review workflow

Follow this reasoning internally.

### 1. Infer the page's user need

Determine why someone would reasonably open this page.

Look at the title, introduction, headings, actions, assumptions about the
reader, and the content itself.

Try to express the need plainly, for example:

- configure session timeout;
- learn how deployments work;
- look up the parameters of an endpoint;
- learn to create a first project.

If the page appears to serve several substantially different needs, note that.
Do not invent a single purpose merely to make classification easier.

### 2. Use Diátaxis to establish an expectation

Apply the action/cognition and acquisition/application dimensions.

Determine the dominant mode that would best serve the inferred user need.

Do this to establish an expected shape for the page, not merely to attach a
label to it.

Ask what follows from that classification:

- If this is a how-to, is there a coherent real-world goal?
- If this is a tutorial, does it provide a coherent learning experience?
- If this is reference, is the material organized for reliable lookup?
- If this is explanation, does it build understanding around a bounded topic?

### 3. Compare the actual page with that expectation

Inspect how the page is put together.

Look especially for problems such as:

- **Unclear purpose** — the page does not make clear what user need it serves.
- **Scope that is too broad** — several independently useful tasks or subjects
  have been bundled into one page without a strong reason.
- **Task-boundary problems** — setup, administration, execution, maintenance,
  troubleshooting, or other distinct jobs are combined in a way that makes the
  user's path harder to follow.
- **Audience or role mismatch** — different sections assume substantially
  different permissions, knowledge, responsibilities, or goals.
- **Structural mismatch** — the organization of the page does not match how
  the user needs to work, learn, look information up, or build understanding.
- **Mode mismatch** — the page is shaped like one kind of documentation while
  the user's actual need calls for another.
- **Mode conflict** — material serving a different Diátaxis need substantially
  interrupts or competes with the page's dominant purpose.
- **Poor placement of supporting material** — useful prerequisites, reference
  details, explanation, warnings, or examples appear where they distract from
  rather than support the main purpose.

These are diagnostic possibilities, not boxes that must all be checked.

A problem does not need to be a Diátaxis mode conflict to matter.

### 4. Judge whether the page is coherent

Consider the page as a whole.

Ask:

- Is there a clear reason for this page to exist?
- Would the intended user recognize that reason?
- Does the page mostly serve that need?
- Does its scope make sense for that need?
- Does the sequence and grouping of information help the user?
- Are different tasks, roles, or modes combined for a useful reason, or merely
  because they concern the same product or feature?

Do not equate "about the same feature" with "belongs on the same page."

Conversely, do not split content merely because it contains different roles,
interfaces, sub-actions, or Diátaxis modes. Keep them together when they form a
coherent experience for the user.

### 5. Find the highest-value problem

Identify the problem that most weakens the page's ability to serve its user.

Do not produce a backlog of every possible improvement.

Prefer the structural issue that explains the largest amount of friction.

If the page is already coherent and appropriate for its purpose, say so rather
than inventing a problem.

### 6. Recommend one next improvement

Recommend the smallest practical change that would meaningfully improve the
page.

Depending on the diagnosis, this might mean:

- split one independent task into another page;
- move background explanation elsewhere and link to it;
- bring a prerequisite closer to the task it affects;
- narrow or clarify the page's purpose;
- reorganize sections around the user's workflow;
- separate content intended for substantially different roles;
- turn a feature catalogue into task-oriented pages;
- restructure reference material for lookup;
- remove material that does not serve the page's purpose.

Explain why the change follows from the user need.

If the user asks to apply the recommendation, make only that focused change
unless they explicitly request a broader rewrite.

## Distinguishing supporting content from real conflict

Documentation does not need to be perfectly pure.

A how-to can contain parameter definitions, constraints, expected results, or
short explanations. A tutorial can contain reference facts. Reference can
include examples. Explanation can point to practical procedures.

Treat cross-mode material as a problem only when it meaningfully interferes
with the dominant user need.

For example, field definitions inside a configuration step are usually useful
supporting reference material. They do not automatically justify moving the
material to a separate reference page.

The presence of another Diátaxis mode is evidence to inspect, not automatically
a reason to split content.

## Guardrails

- Evaluate one page or small fragment at a time unless the user explicitly asks
  for a broader information-architecture review.
- Do not force documentation into four top-level sections. Diátaxis describes
  user needs and documentation forms, not a mandatory site structure.
- Do not assume every page must contain exactly one action, role, or interface.
  Judge whether the material forms a coherent whole for the user.
- Do not call multiple roles, goals, or interfaces a Diátaxis mode conflict
  unless they genuinely represent competing documentation needs.
- Do not confuse tutorial vs how-to with beginner vs advanced. The distinction
  is learning versus performing real work.
- Do not confuse reference vs explanation with short versus long. The
  distinction is consultation during work versus developing understanding.
- Do not treat classification as the outcome of the review. Use it to reason
  about what the page should do.
- Do not grade Diátaxis compliance numerically.
- Do not claim to verify factual accuracy, technical correctness,
  completeness, accessibility, SEO, grammar, or prose style unless the user
  separately asks for those checks and provides enough evidence.
- Do not turn a page review into a comprehensive documentation redesign.
- Do not recommend splitting content merely to achieve mode purity.
- Do not invent problems when the page already serves its purpose well.

## Output

Write concise, natural editorial feedback rather than a diagnostic form.

Start with the main conclusion about the page: what it appears to help the user
do or understand, and whether the page is coherently built around that need.

Explain the most important structural problem using concrete evidence from the
page. Then recommend one practical next improvement and explain why it would
better serve the user.

Use Diátaxis terminology when it makes the reasoning clearer, but do not force
the response into fields such as "Dominant mode", "User need", "Mode conflict",
or confidence levels.

A useful review often sounds like:

> This is fundamentally a how-to, but the page combines the configuration of
> the feature with the task of using it. Those jobs belong to different users
> and happen at different moments, so someone who only wants to perform the
> task has to work around setup material they may not even have permission to
> use.
>
> I would move the administrative setup into its own how-to and leave this page
> focused on the user action, with a short prerequisite linking to the setup
> instructions.

The reasoning comes from Diátaxis, but the feedback should describe the actual
documentation problem.

If the user explicitly asks for classification, a formal Diátaxis audit, or an
explanation of the reasoning, provide the underlying mode and compass analysis.

## Examples

### Several how-to tasks on one page

A page called **Visual Workflow Editor** explains how to install the editor,
connect it to a portal, navigate its canvas, create and remove statuses, manage
transitions, validate a workflow, import and export JSON, and apply changes.

Do not manufacture a reference/how-to conflict merely because some sections
define fields or describe interface behavior.

Instead reason from the user need:

The content is predominantly action-oriented work, but the page does not have
a sufficiently clear task boundary. It acts as a collection of several
independently useful how-to tasks simply because they concern the same tool.

Recommend the highest-value structural separation, such as extracting an
independent task or establishing a clear main workflow and moving optional
operations to their own pages.

### Genuine mode conflict

A page called **Rotate an API key** gives the steps needed to replace a key,
but between the steps contains several paragraphs explaining the history of
the authentication model, why the product uses tokens, and alternative
authentication architectures.

The user's need is to complete a real-world task, so the expected mode is
how-to.

The explanatory material serves a different need and interrupts the task
without being necessary to complete it. Recommend moving the deeper
explanation to a separate explanation page and linking to it where useful.

The problem is not that explanation appeared inside a how-to. The problem is
that it competes with the user's immediate purpose.