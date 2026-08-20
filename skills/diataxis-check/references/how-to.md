# How-to diagnostic model

Use this reference when the intended reader is applying existing competence
through action: the reader is at work and needs help accomplishing a
real-world task, goal, project, or problem.

A how-to guide is defined by the reader's practical project, not by the
product feature used to accomplish it.

## Establish the human project

Identify the result the reader is trying to achieve.

Express it as a human task or problem, not merely as a product operation.

Prefer:

- configure session timeout for an organization;
- rotate credentials without interrupting service;
- publish a workflow change;
- recover a failed deployment.

Be suspicious of scopes that merely reproduce product capabilities:

- Statuses
- Transitions
- Validation
- Import
- Export
- Settings

Those sections may all be valid product concepts, but they do not establish a
single how-to guide.

Ask what reader project makes them belong together.

## Let the project define scope

The reader's project determines what the guide must cover.

A how-to may stay inside one feature when the task naturally aligns with that
feature.

It may also cross:

- several features;
- several interfaces;
- several tools;
- several technical subsystems;

when accomplishing the reader's goal requires them.

Do not force how-to boundaries to match product boundaries.

Conversely, several operations do not belong on one page merely because the
same feature exposes them.

If sections have independent entry points, outcomes, or moments of use, check
whether they are actually separate how-to tasks.

## Do not narrate the machinery

Instructions can look procedural while providing little task guidance.

Flag steps that merely tell a competent reader to operate an obvious control
for its obvious effect when that information does not help solve the reader's
problem.

For example, the useful question may be:

> Which option should I use in this situation?

rather than:

> Where is the option and how do I click it?

The product is normally a means to the reader's end.

Do not treat operation of the product as a meaningful goal by itself unless
that operation really is the reader's project.

## Assume relevant competence

A how-to guide serves a reader who is already able to work in the domain.

Do not require it to teach foundational competence merely because some readers
might lack it.

The guide can normally assume familiarity with ordinary tools, terminology,
and basic operations appropriate to the task.

Need for detailed guidance does not imply lack of competence.

An expert may still consult a detailed how-to to make sure a task is performed
correctly.

If the page spends substantial effort creating foundational competence, check
whether tutorial material has entered the guide.

## Represent real-world variability

A how-to guide operates in real work, where the writer cannot control all
conditions in advance.

Do not require every valid how-to to be one rigid linear procedure.

Check whether the real task includes:

- different starting conditions;
- conditional branches;
- alternative valid routes;
- exceptions;
- known disruptions;
- decisions;
- practitioner judgement.

When such variation materially affects the task, the guide should expose
enough decision logic for a competent reader to choose an appropriate route.

Do not solve this by enumerating every theoretically possible case.

The goal is adaptable guidance, not exhaustive case coverage.

## Check the sequence against the work

A how-to still needs a meaningful progression.

Do not evaluate the sequence from an abstract claim that "the order should
make sense."

Check concrete ordering constraints.

### Dependencies

If one action requires another to have happened first, the guide should reflect
that dependency.

Flag prerequisites introduced after the reader already needed them.

### Preparation

Even when two actions are technically interchangeable, one may need to appear
first because it prepares:

- the working environment;
- information needed for a later decision;
- the reader's understanding of the immediate task.

Do not reorder steps without evidence from the task.

### Context switching

Flag repeated switching between tools, interfaces, roles, or unrelated
concerns when the switching results from page organization rather than from
the task itself.

### Unresolved decisions

Flag information or decisions introduced substantially before the reader can
act on them when that forces the reader to remember unresolved concerns across
many intervening steps.

### Backtracking

Inspect jumps back to an earlier concern.

Backtracking is not automatically wrong.

Treat it as a structural problem when it exists only because the guide
introduced or ordered material badly.

### Information timing

Place prerequisites, warnings, decision criteria, and supporting facts near
the point where the reader needs them.

Do not require all prerequisites or background information to appear at the
top when doing so separates them unnecessarily from their use.

## Prefer practical usability over exhaustive coverage

A how-to does not need to cover the reader's complete end-to-end workflow.

It may begin from a meaningful existing state and stop when the stated task has
been accomplished sufficiently.

A competent reader can join the guide to surrounding work.

Do not use this principle to excuse gaps inside the task the page claims to
solve.

The documented route still needs to provide a viable solution for the stated
situation.

## Distinguish how-to from tutorial

Both modes guide action.

Use work versus study as the decisive distinction.

A how-to:

- assumes relevant competence;
- serves an actual task;
- can rely on implicit familiarity;
- operates under real-world conditions;
- may branch;
- can require practitioner judgement;
- cannot fully manage what happens.

A tutorial:

- creates competence;
- constructs a learning experience;
- deliberately familiarizes the learner with tools and processes;
- controls conditions where possible;
- minimizes choices;
- carries more responsibility for the reader's successful path.

Do not classify by difficulty.

Do not assume detailed steps imply tutorial.

Do not assume an experienced reader can never be in a tutorial situation.

## Use supporting material only when it helps the work

A how-to can contain:

- concise parameter information;
- constraints;
- warnings;
- expected results;
- brief reasons;
- small examples.

Do not classify these automatically as mode conflicts.

Treat supporting material as a problem when it:

- interrupts progress toward the task;
- grows into an exhaustive catalogue;
- requires the reader to stop working and study another subject;
- exists mainly because the author wants the page to be complete;
- becomes an independently useful reference or explanation.

Link to deeper material when it is important but not part of the task flow.

## Check the title and opening

The reader should be able to identify the practical problem or result the page
addresses.

A bare topic title such as:

> Application performance monitoring

does not establish a how-to purpose.

A page title does not need to use the literal words "How to", but it should
make the task sufficiently clear.

Do not classify from title alone; use it as evidence about intended scope.

## Diagnostic questions

Ask:

- What practical result is the reader trying to achieve?
- Can the result be described without merely naming a feature?
- Does that project determine the page's scope?
- Are major sections together because the task needs them together?
- Are independent tasks bundled because they share a product area?
- Does the guide explain useful decisions rather than merely narrate controls?
- Does it assume appropriate working competence?
- Does it accommodate real variation that materially affects the task?
- Has real branching been forced into a false linear procedure?
- Are dependencies represented in the correct order?
- Are prerequisites introduced before they are needed?
- Does the page create avoidable context switching?
- Does it introduce decisions too early?
- Does it cause avoidable backtracking?
- Is supporting information located near its use?
- Is exhaustive coverage interfering with practical usability?

## Common structural failures

### Feature tour disguised as how-to

The page enumerates product operations without a coherent human project.

### Several independent tasks on one page

Each section is useful, but the sections solve different problems or are used
at different moments.

### Obvious interface narration

The guide describes controls that a competent reader can already operate
without connecting those actions to a real-world decision or outcome.

### Tutorial material inside work guidance

The page teaches basic competence instead of supporting application of
existing competence.

### Artificially linear guidance

The task requires conditional reasoning or alternative routes, but the guide
pretends one procedure fits every real case.

### Exhaustive product coverage

Options, background, and feature information accumulate because they concern
the same product area rather than because the reader needs them for the task.

### Broken work sequence

The page causes late prerequisites, avoidable switching, premature decisions,
or unnecessary backtracking.

## Recommendation patterns

Prefer one change that reconnects the page with the reader's real work, for
example:

- redefine the page around one concrete project;
- split an independent task into its own guide;
- reorganize feature-oriented sections around the reader's workflow;
- remove obvious interface narration;
- add decision guidance for a real-world branch;
- move exhaustive option information to reference;
- move extended conceptual discussion to explanation;
- reorder a late prerequisite;
- move a decision closer to the point where it is needed;
- reduce avoidable context switching or backtracking.

Do not redesign the guide merely to make it mode-pure.

Judge whether a competent reader can use it effectively to accomplish the
real-world task.