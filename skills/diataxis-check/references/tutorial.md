# Tutorial diagnostic model

Use this reference when the intended reader is acquiring skill or knowledge
through action: the reader is at study and needs a guided learning experience.

A tutorial is a lesson. Its practical activity is the means by which learning
happens; completing the activity is not necessarily the ultimate purpose.

## Establish the learning purpose

Distinguish:

- what the learner does;
- what the learner is meant to acquire by doing it.

For example, creating and deploying an application can be the activity while
the intended learning concerns tools, workflow, terminology, relationships,
commands, or system behavior.

Do not judge a tutorial only by whether the final artifact works.

Ask what competence or familiarity the complete experience is intended to
develop.

If successful completion of a real-world task is itself the primary purpose,
the page is more likely serving a how-to need.

## Treat the page as a managed learning experience

The tutorial carries much more responsibility for the reader's path than a
how-to guide does.

Check whether an attentive learner can follow the documented path without
having to:

- invent missing steps;
- choose among alternatives they cannot yet evaluate;
- diagnose predictable failures unaided;
- know in advance which details matter;
- make decisions that require competence the tutorial is supposed to develop.

The learner may not yet know which questions to ask.

Do not make the learner design their own learning path.

## Check what the learner encounters

A tutorial should deliberately expose the learner to the actions, concepts,
tools, terminology, processes, and behavior required by the intended learning.

Do not require exhaustive product coverage.

Instead, check whether the chosen learning journey includes the encounters
needed for its learning purpose.

A tutorial can be incomplete even when every documented instruction works, if
an important encounter needed for the intended learning never occurs.

Conversely, unrelated product features do not belong merely for completeness.

## Keep the path concrete

Tutorial learning should be anchored in specific actions, objects, and visible
results.

Check for:

- long conceptual introductions before the learner does anything;
- general abstractions replacing concrete experience;
- explanations that make the learner stop following the activity;
- large jumps that require the learner to infer intermediate actions.

Prefer a progression from concrete experience toward broader understanding,
rather than requiring abstract understanding before the learner can begin.

Do not add abstraction merely because an expert naturally thinks about the
subject abstractly.

## Check action-result feedback

A learner repeatedly needs to know whether they are still on the correct path.

For significant actions, check whether the tutorial gives enough evidence to
recognize success.

Useful evidence can include:

- visible state changes;
- expected output;
- exact output where appropriate;
- a result the learner can compare with;
- a warning that an unusual result is actually expected;
- a known failure sign and its likely cause.

Do not wait until the end of the tutorial to confirm that the learner has been
successful.

When the result of an action matters to later steps, ambiguity about that
result is especially serious.

## Point out what the learner should notice

An observable effect is not automatically a learning encounter.

Learners can be too focused on performing a new action to notice something
important that happens around it.

When an observation matters to the intended learning, point it out at the time
it becomes visible.

Keep the cue brief enough that it does not turn into a separate explanatory
discussion.

## Minimize unnecessary choices

A tutorial normally chooses a workable path for the learner.

Flag alternatives when the learner is asked to choose between:

- tools;
- architectures;
- configurations;
- equivalent commands;
- optional approaches;

without the competence needed to evaluate them.

Do not interpret this as a rule that tutorials can never contain a branch.

A branch may be necessary to recover from a known condition or to keep the
learning experience working.

The problem is unnecessary choice that transfers responsibility for designing
the learning path to the learner.

## Control avoidable variability

A tutorial normally uses known tools, conditions, values, and starting states
so that the learning experience can be made reliable.

Check whether ordinary variation has been left uncontrolled when the tutorial
could reasonably specify it.

For example, an introductory software tutorial may need to choose:

- one operating path;
- one configuration;
- one example dataset;
- one known version;
- one concrete set of values.

The purpose is not to model every real-world case.

It is to create a successful encounter from which competence can develop.

## Protect learner confidence

A tutorial should give the learner repeated evidence that following the
instructions produces the promised results.

Treat a broken action/result expectation as significant.

Written documentation cannot observe the learner and intervene like a live
teacher.

Where predictable confusion or failure is known, the tutorial should normally
anticipate it instead of relying on the learner to recover independently.

## Consider repetition where it helps learning

Repeated successful action can build familiarity and confidence.

Where practical, check whether important operations can be repeated without
rebuilding the entire environment.

Do not make repeatability an absolute requirement when the operation is
inherently irreversible.

The diagnostic question is whether a one-off design unnecessarily prevents the
learner from practising something that benefits from repetition.

## Distinguish tutorial from how-to

Both tutorial and how-to contain action.

Use study versus work as the primary distinction.

A tutorial:

- creates competence;
- manages the learning path;
- deliberately familiarizes the reader with tools and processes;
- can make basic interactions explicit;
- controls conditions where possible;
- minimizes unnecessary choice;
- carries substantial responsibility for successful progression.

A how-to guide:

- assumes relevant competence;
- supports real work;
- can rely on familiarity and practitioner judgement;
- must accommodate real-world variation;
- may branch according to conditions;
- cannot control the reader's situation in the same way.

Do not use beginner versus advanced as the distinction.

An expert studying an unfamiliar technique can need a tutorial.

A relatively simple production task can still need a how-to guide.

## Keep explanation subordinate to the learning experience

A short explanation can support a tutorial when the learner needs it to make
sense of the current action.

Extended explanation is suspect when it interrupts the action-result learning
loop.

If removing an explanatory passage reveals that the learner can no longer
proceed without guessing, do not simply restore the explanation.

Check whether the tutorial has concealed a missing instructional step or
learning transition.

Move deeper conceptual treatment elsewhere when it represents an independent
understanding need.

## Diagnostic questions

Ask:

- What is the learner meant to acquire?
- What activity creates that learning opportunity?
- Does the practical outcome serve learning, or has it become the real goal?
- Can the learner see what they are working toward?
- Does the learner encounter everything needed for the intended learning?
- Is the path sufficiently controlled for an attentive learner to succeed?
- Are unnecessary choices delegated to the learner?
- Do important actions produce recognizable results?
- Are expected results shown where uncertainty would otherwise remain?
- Are important observations pointed out when they occur?
- Is the learner required to infer missing actions or decisions?
- Does explanation interrupt the concrete learning experience?
- Does the path build or undermine confidence?

## Common structural failures

### Procedure mistaken for lesson

The page contains detailed steps but merely gets a reader through a task. The
task is the end rather than the vehicle for learning.

### Information substituted for experience

The page explains or describes extensively while the learner has little
meaningful activity.

### Learner carries the teacher's responsibility

The page requires troubleshooting, path selection, or domain decisions that
the learner is not yet equipped to make.

### Missing feedback

The learner performs important actions but cannot tell whether the expected
state has been reached.

### Missing learning encounter

The final task succeeds, but the path never exposes the learner to something
the intended competence requires.

### Unnecessary alternatives

The tutorial turns into a menu of possible approaches instead of providing one
managed learning path.

### Explanation hides an instructional gap

Conceptual prose appears to connect two steps, but after removing it the
learner is left to work out what to do next.

## Recommendation patterns

Prefer one change that improves the learning experience directly, for example:

- clarify the competence the tutorial is meant to develop;
- establish a concrete achievable outcome;
- repair a missing action or transition;
- add an expected result after an important action;
- point out an observation the learner currently misses;
- remove an unnecessary choice;
- specify a condition that is currently left uncontrolled;
- move extended explanation out of the learning path;
- add a missing encounter with an important tool or concept;
- narrow the tutorial so the chosen path can be made reliable.

Judge the tutorial by the quality of the guided learning experience, not by the
amount of information it contains.