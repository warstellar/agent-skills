---
name: decision-log
description: Maintain a lightweight DECISIONS.md log of durable, material decisions in persistent agent workspaces. Use when a decision has actually been made and preserving its rationale would matter to future work, especially when it changes or clarifies prior requirements, structure, workflows, conventions, strategy, or other lasting assumptions. Applies to software projects, product and design work, research, knowledge bases, and other persistent workspaces. Do not use for routine execution choices, cleanup, formatting, naming, transient fixes, or brainstorming before a decision is made.
license: MIT
metadata:
  author: Ian Corvin
  version: "0.1.0"
---

# Decision Log

Preserve the reasoning behind consequential decisions so future humans and agents can understand why a workspace evolved the way it did.

Use `DECISIONS.md` as lightweight project memory, not as a changelog or a record of everything that happened.

## Workflow

When a decision emerges during work:

1. Wait until a decision has actually been made. Do not log ideas, open questions, or alternatives that are still being explored.
2. Apply the decision gate below.
3. If the decision does not pass the gate, continue the work without mentioning the decision log.
4. If it passes, locate an existing `DECISIONS.md` in the relevant workspace.
5. If no decision log exists, propose creating `DECISIONS.md`. Do not create one proactively before the first qualifying decision.
6. Once a decision log exists, record future qualifying decisions as part of the work without asking for confirmation each time, unless the user has requested otherwise.
7. Put new decisions at the top of the log, immediately below its introductory text.

Do not interrupt work merely to search for something worth recording. Decisions should emerge from the work; never manufacture decisions to justify using this skill.

## Decision gate

Automatically record a decision only when it passes all of these tests:

**Durable**  
The choice is expected to affect future work, not only the current action.

**Material**  
The choice meaningfully changes, establishes, rejects, or clarifies a direction, assumption, rule, structure, workflow, behavior, responsibility, or constraint.

**Rationale matters**  
If the outcome remained but its reasoning disappeared, a future person or agent could reasonably question it, reverse it, repeat the same discussion, or incorrectly restore an earlier assumption.

When in doubt, do not record. A missing marginal decision is better than a noisy decision log.

An explicit user request to record a decision overrides the automatic decision gate.

Treat phrases such as "record this decision", "log this", "let's capture this",
or equivalent requests as explicit intent to add the decision to the log.

## What not to record

Do not record routine execution choices merely because a choice was made.

Examples include:

- file moves and cleanup;
- formatting and cosmetic adjustments;
- ordinary naming choices;
- routine dependency updates;
- straightforward bug fixes;
- refactoring that does not materially change behavior or structure;
- local implementation details that naturally follow from an existing decision;
- temporary operational choices with no expected lasting effect;
- actions taken solely to complete the current task.

The amount of thought required does not make something a durable decision.

For example, deciding where cleaned-up files from `Downloads` should go is not a project decision unless it establishes a meaningful, lasting workspace convention whose rationale will matter later.

## `DECISIONS.md` format

If creating the file, start with:

```markdown
# Decisions

Significant decisions that shape future work and explain why this workspace evolved the way it did.

Newest decisions first.
```

Use this structure for each decision:

```markdown
## YYYY-MM-DD — Short decision title

### Decision

State what was decided. Lead with the outcome, not the history of the discussion.

### Context

Explain why a decision became necessary.

Include relevant prior assumptions, requirements, evidence, problems, discoveries, or earlier decisions when they are important for understanding what changed.

### Reasoning

Explain why this option was chosen.

Mention meaningful alternatives only when they were actually considered. Do not invent alternatives to make the record look complete.

### Trade-offs

Include only when there are concrete drawbacks, risks, constraints, or capabilities knowingly given up.
```

`Trade-offs` is optional. Omit the section when there is nothing useful to say.

Keep entries concise. Preserve enough context to recover the reasoning, but do not reproduce the entire discussion.

Do not fill sections with generic statements merely to complete the template.

## Existing decisions

Treat previous decision entries as historical records.

When a later decision reverses, replaces, or substantially changes an earlier one:

- add a new decision rather than silently rewriting the old reasoning;
- mention the previous decision naturally in `Context`;
- explain what changed since it was made.

Edit an old entry only to fix a clear factual or formatting error, not to make history agree with the current state.

## Examples

### Record

A product specification assumes that every task should start automatically. During real use, this creates unexpected work and removes user control. The team decides that task creation and task execution must be separate actions.

This is durable, material, and the rationale matters.

### Record

A personal knowledge workspace organizes information primarily by topic. Repeated use shows that information is duplicated across topics, so the workspace switches to project-centered organization.

This changes a lasting structural convention and should be recorded.

### Record

A research workflow originally keeps source summaries only. After discovering that later agents cannot reliably distinguish evidence from interpretation, the workspace adopts a rule that important claims must retain source references.

This establishes a lasting workflow rule whose reason may not be obvious later.

### Do not record

An agent moves files out of `Downloads` after completing a cleanup.

This is an execution detail, not a material workspace decision.

### Do not record

A component is renamed to better match the surrounding naming convention.

The result may persist, but its rationale is unlikely to matter to future work.

### Do not record

Several implementation approaches are discussed, but no direction has been chosen yet.

The decision log records decisions, not brainstorming.