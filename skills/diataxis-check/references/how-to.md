# How-to diagnostic model

Read this file after `SKILL.md` has inferred that the intended documentation
reader primarily needs to act while applying existing competence: the reader is
doing real work and wants to achieve a practical result.

Use this as diagnostic guidance for reviewing a page. It is not a complete
writing guide for creating how-to documentation from scratch.

## Reader situation

A how-to guide serves a reader who:

- already has enough competence to work in the domain;
- knows what they are trying to accomplish;
- faces a real task, problem, project, or desired result;
- needs guidance that helps them move through that real-world situation.

The reader's project defines the guide.

The product, feature, interface, API, command, or tool is normally a means to
that end, not the reason the guide exists.

## Expected content architecture

A good how-to guide:

- addresses a recognizable real-world goal or problem;
- is organized from the reader's perspective rather than the machinery's;
- includes actions that help reach the desired result;
- assumes ordinary competence instead of teaching fundamentals;
- accommodates conditions, branches, judgement, and variation when the real
  task requires them;
- starts and ends at meaningful points in the reader's work;
- prefers practical usefulness over exhaustive coverage;
- orders actions according to the logic of the reader's work and thinking;
- maintains flow by avoiding unnecessary detours and context switches;
- makes clear what practical problem or outcome it addresses.

A how-to does not need to be a rigid linear procedure.

Real work can branch, overlap, have multiple entry and exit points, and require
judgement.

## User goal versus product structure

Pay special attention to what determines the page's structure.

A page organized as:

- Statuses
- Transitions
- Validation
- Import
- Export
- Settings

may simply mirror the capabilities or structure of a tool.

That can be appropriate for reference.

For a how-to, ask what reader project makes those sections belong together.

A good how-to may cross several screens, features, tools, or subsystems when
the reader's goal requires it.

Conversely, several operations in the same feature do not automatically form
one coherent how-to.

The key question is not:

> What can this feature do?

It is:

> What is the reader trying to get done?

## Diagnostic questions

Ask:

- What concrete result is the reader trying to achieve?
- Can that result be described as a human task or problem rather than merely as
  operating a feature?
- Is the page organized around that result?
- Does every major section help advance the same reader project?
- Are several independent tasks grouped together merely because they use the
  same product area?
- Does the guide begin where this reader reasonably needs guidance?
- Does it stop when the practical task has been sufficiently served?
- Are prerequisites relevant to this reader and this task?
- Does the sequence follow the reader's work and thinking?
- Does the page force unnecessary switching between roles, tools, contexts, or
  concerns?
- Is material included because it helps the reader act, or merely for
  completeness?
- Where real situations vary, does the guidance allow enough branching or
  judgement to remain useful?

## Common failure patterns

### Feature tour disguised as how-to

The page enumerates things that can be done with a product or interface without
connecting them to a meaningful reader goal.

The operations may all be valid.

Their shared relationship to the product does not establish a shared reader
task.

### Several independent tasks on one page

Each section solves a useful practical problem, but the sections have different
entry points, outcomes, or moments in the reader's work.

The page becomes a collection of how-to guides rather than one coherent guide.

### Setup mixed with routine work

Installation, initial configuration, permissions, or administration is embedded
inside a task performed repeatedly by another reader or at another stage.

Treat this as a problem when setup interrupts the normal work rather than
serving as a concise prerequisite.

### Instructions without meaningful purpose

The page tells an already-competent reader how to operate obvious controls or
move the system through its motions without connecting those actions to a
real-world problem.

### Completeness over usability

Options, background facts, feature descriptions, and edge cases accumulate
because the author wants the page to cover everything related to the feature.

A how-to needs enough information to be useful in real work, not everything
that can be said about the machinery.

### Broken flow

The ordering may be technically valid but poorly aligned with the reader's
actual work.

Look for:

- unnecessary context switching;
- jumping back to earlier concerns;
- prerequisites discovered too late;
- information that must be remembered for too long before it becomes useful;
- sequences organized for the system rather than for the reader.

## Supporting content and boundaries

Reference facts, constraints, warnings, expected results, and short
explanations can support a how-to when they help the reader make progress.

Their presence is not automatically a mode conflict.

Treat supporting material as a problem when it:

- interrupts progress toward the practical goal;
- exists mainly for completeness;
- asks the reader to stop working and study a different subject;
- grows large enough to represent an independent information or understanding
  need.

Link to deeper reference or explanation when appropriate.

## Recommendation patterns

Prefer recommendations that restore the connection between the page and the
reader's real work.

Depending on the diagnosis, recommend one high-value change such as:

- redefine the page around a concrete reader goal;
- split independent tasks into separate how-to guides;
- reorganize sections around the reader's workflow rather than feature
  categories;
- move one-time setup out of a recurring task;
- remove obvious system-operation detail that does not help solve the problem;
- move exhaustive reference information elsewhere;
- reorder actions to improve flow;
- clarify the title so it states the task or outcome.

Do not recommend changes merely to make the page more mode-pure.

The criterion is whether the guide helps a competent reader accomplish the
real task effectively.