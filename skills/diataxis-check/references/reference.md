# Reference diagnostic model

Read this file after `SKILL.md` has inferred that the intended documentation
reader primarily needs cognition while applying existing knowledge: the reader
is working and needs reliable information to consult.

Use this as diagnostic guidance for reviewing a page. It is not a complete
reference-authoring standard.

## Reader situation

Reference serves a practitioner who:

- is already engaged in work;
- knows roughly what information they need;
- needs facts about a product, system, API, command, object, option, or other
  machinery;
- expects to find the information quickly;
- expects to be able to rely on what they find.

Reference is consulted rather than followed as a journey.

Unlike tutorials and how-to guides, reference is normally led by the structure
of the thing being described rather than by a human project.

## Expected content architecture

Good reference:

- describes the machinery clearly and authoritatively;
- states facts, behavior, constraints, options, parameters, relationships,
  limitations, and warnings;
- uses neutral and factual language;
- is organized predictably;
- follows consistent patterns;
- mirrors the logical or conceptual structure of the system where that helps
  readers navigate it;
- makes relevant information easy to locate;
- uses examples when they efficiently illustrate the thing being described;
- avoids becoming a task guide or conceptual discussion.

Its primary job is dependable description.

## Product structure can be the right structure

Reference is the Diátaxis mode in which product-oriented organization is often
appropriate.

Sections such as:

- endpoints;
- classes;
- commands;
- configuration fields;
- object properties;
- status types;
- events;
- error codes

may be useful precisely because the documentation reflects the machinery the
reader needs to inspect.

Do not automatically criticize reference for being feature-oriented.

Instead ask whether the structure helps a working reader locate and understand
the relevant facts.

Consistency matters strongly.

Similar things should expose similar kinds of information in similar places.

## Diagnostic questions

Ask:

- What thing or system element is this page describing?
- Would a working reader come here mainly to look something up?
- Does the page provide dependable facts rather than guide a particular
  project?
- Is the scope aligned with a meaningful part of the machinery?
- Does the organization make information easy to locate?
- Does the documentation structure correspond sensibly to the system's
  structure?
- Are similar entities documented using predictable patterns?
- Are important properties, constraints, behavior, values, and warnings easy
  to distinguish?
- Is the page drifting into instructions for an independent real-world task?
- Is it drifting into reasons, history, trade-offs, interpretation, or broader
  conceptual discussion?
- Do examples illustrate the described machinery, or quietly become tutorials
  or how-to guides?

## Common failure patterns

### Task guidance embedded in reference

The page begins by describing an object, feature, or API but turns into
instructions for accomplishing a particular reader goal.

That task may deserve a how-to guide that links back to the reference.

### Explanation embedded in reference

History, rationale, alternatives, interpretation, or conceptual discussion
expands around factual description.

That material may be valuable, but it serves understanding rather than lookup.

### Inconsistent structure

Related entities expose similar information under different headings, in
different orders, or in different formats.

This makes consultation slower and less predictable.

### Structure that obscures the machinery

Information is grouped according to arbitrary prose themes even though readers
navigate the underlying system through clear entities, categories, or
relationships.

### Description becomes commentary

Facts are mixed with persuasion, speculation, unnecessary judgement, or
discursive interpretation.

Reference should give the reader confidence about what the machinery is and
does.

### No clear place for important facts

The page's architecture makes it difficult to locate obvious categories of
information such as:

- possible values;
- parameters;
- constraints;
- behavior;
- warnings;
- relationships;
- limitations.

Do not use this observation to claim factual completeness or incompleteness
without sufficient evidence.

The diagnosis is about whether the structure supports reference use.

## Supporting content and boundaries

Reference can contain:

- concise usage examples;
- short descriptions of correct use;
- warnings;
- limited contextual notes needed to understand a fact.

These do not automatically turn the page into another mode.

The boundary is crossed when the page substantially begins to:

- lead the reader through a real-world project;
- teach a learner through a guided experience;
- develop a broader conceptual understanding.

## Recommendation patterns

Prefer recommendations that improve consultation and predictability.

Depending on the diagnosis, recommend one high-value change such as:

- reorganize the page around the logical structure of the machinery;
- introduce consistent patterns for related entities;
- separate a task-oriented procedure into a how-to guide;
- move extended rationale or conceptual discussion to explanation;
- replace discursive prose with clearer factual structure;
- make important properties, constraints, or warnings easier to find;
- add concise examples that illustrate usage without becoming a tutorial.

Do not reorganize reference around reader goals merely because goal-oriented
organization is valuable in how-to documentation.

Product-led structure is a strength of reference when it helps readers consult
the machinery efficiently.