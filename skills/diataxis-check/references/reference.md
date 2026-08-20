# Reference diagnostic model

Use this reference when the intended reader needs theoretical or propositional
knowledge while applying existing competence: the reader is at work and needs
reliable information to consult.

Reference primarily describes the machinery.

It is not organized around one particular reader project.

## Establish the lookup need

Ask what information the working reader needs to know.

Typical reference subjects include:

- APIs;
- endpoints;
- classes;
- methods;
- commands;
- configuration fields;
- flags;
- properties;
- values;
- events;
- error codes;
- constraints;
- system behavior.

The same reference information can support several different reader tasks.

Do not require the page to be organized around one of those tasks merely
because the information will be used during work.

## Distinguish description from task guidance

Reference can describe:

- what something is;
- what it does;
- how it behaves;
- what values it accepts;
- what constraints apply;
- how it is correctly used.

Describing correct use does not automatically make content a how-to guide.

The boundary is crossed when the material begins leading the reader through a
human project.

Compare:

> `timeout` accepts values from 30 to 3600 seconds.

with:

> To reduce idle sessions across your organization, first change the global
> timeout, then...

The first describes the machinery.

The second begins guiding a task.

## Let the machinery help define scope

Reference is legitimately product-led.

The technical object being described can determine the page's scope and
organization.

Check whether meaningful relationships in the system are reflected in the
documentation.

For example:

- related commands can share a predictable structure;
- properties can appear under the objects they belong to;
- API resources can reflect meaningful API relationships.

Do not convert reference into task-oriented organization simply because
reader-centered organization is appropriate for how-to guides.

## Do not mirror implementation mechanically

"Follow the machinery" does not mean reproducing every internal implementation
detail.

Use logical and conceptual relationships that help the reader understand and
navigate the documented system.

Flag literal implementation mirroring when it creates an unnatural structure
for the documented technical surface.

The goal is correspondence that helps consultation, not duplication of source
code layout.

## Optimize for consultation

Reference is normally consulted rather than read as a narrative.

Check whether a reader can locate a particular fact without reading the page
from the beginning.

Use predictable structure.

For related entities, check whether equivalent kinds of information appear:

- under consistent headings;
- in a consistent order;
- using consistent terminology;
- in familiar formats.

Do not introduce structural or vocabulary variation merely for stylistic
variety.

Predictability is a feature of reference.

## Separate authoritative facts from interpretation

Reference should make it clear what the documented technical reality is.

Flag material that makes the reader separate facts from:

- opinion;
- speculation;
- persuasion;
- marketing;
- extended interpretation;
- discursive argument.

This does not mean every sentence must sound identical or artificially terse.

The diagnostic issue is whether authoritative information remains direct and
unambiguous.

## Treat normative language correctly

Words such as:

- must;
- must not;
- never;
- required;

do not automatically indicate how-to instruction.

They are appropriate in reference when they state actual requirements,
constraints, valid states, or rules of correct use.

Classify the function of the statement, not its grammatical mood.

## Use examples as illustration

Examples can belong in reference.

A good reference example makes the described technical element easier to
recognize or understand in context.

Keep an example in reference when it primarily illustrates:

- syntax;
- a value;
- a command;
- a valid structure;
- a concise usage form.

Check for boundary drift when the example expands into:

- a sequence for accomplishing a human goal;
- reasons why the system was designed this way;
- historical development;
- what-if exploration;
- a broader conceptual discussion.

Illustration is compatible with reference.

A task or an explanation is a different reader need.

## Distinguish reference from explanation

Both reference and explanation concern cognition.

Do not decide between them from subject matter alone.

Use the reader's relationship to the work.

Reference serves a reader who needs information while applying knowledge in
work.

Explanation serves a reader who has stepped back from immediate work to study,
reflect, and understand.

Use this test when a factual or conceptual passage could plausibly be either.

Lists and tables are useful reference signals, but they are heuristics rather
than the deciding rule.

## Be cautious about explanatory digressions

A short clarification can support reference.

Treat explanation as a problem when it substantially interrupts consultation.

Typical signs include:

- a factual entry expands into reasons and history;
- a technical definition becomes a conceptual essay;
- the reader must work through interpretation before reaching the needed fact.

This can harm both needs:

- reference becomes slower to consult;
- explanation remains too fragmented to develop properly.

Do not move a one-sentence clarification merely because it has an explanatory
function.

## Functional-quality limits

Reference aspires to accuracy, precision, completeness, clarity, and
reliability.

This skill cannot verify those properties merely by applying Diátaxis.

Do not claim that the reference is accurate or complete unless the supplied
evidence establishes that independently.

Reference structure can expose a possible functional-quality problem.

For example, if several parallel technical entities have predictable entries
and a corresponding entity appears to be absent, flag a possible coverage
gap.

Treat this as evidence to investigate, not proof of incompleteness.

## Diagnostic questions

Ask:

- What machinery or technical object is the reader consulting?
- Does the reader need this information while working?
- Is the page primarily describing rather than guiding a project?
- Does the technical object provide a sensible scope?
- Does the structure reflect meaningful system relationships?
- Has implementation structure been copied too literally?
- Can a reader find individual facts without reading the entire page?
- Are related entities presented consistently?
- Are technical facts clearly distinguishable from interpretation or opinion?
- Are normative statements describing constraints or actually leading a task?
- Do examples illustrate the machinery or become another documentation mode?
- Does explanatory material interfere with lookup?
- Does the structure reveal a possible coverage gap?

## Common structural failures

### Task guidance embedded in reference

The page stops describing the machinery and begins leading one particular
reader project.

### Explanation embedded in reference

Reasons, alternatives, history, or interpretation expand until factual lookup
is interrupted.

### Arbitrary prose organization

Meaningful relationships in the technical object are hidden by an organization
that does not help consultation.

### Mechanical implementation mirroring

Internal code organization is reproduced even when it does not correspond to a
useful reader-facing technical structure.

### Inconsistent patterns

Parallel entities use different headings, terminology, order, or formats.

### Facts mixed with commentary

Opinion, speculation, or promotional language makes authoritative information
harder to identify.

### Example becomes another document

An illustration grows into a complete task or conceptual discussion.

## Recommendation patterns

Prefer one change that improves dependable consultation, for example:

- reorganize the page around meaningful machinery structure;
- standardize parallel entries;
- separate a real task into a how-to guide;
- move extended conceptual discussion to explanation;
- make constraints or properties easier to locate;
- separate authoritative facts from commentary;
- reduce an overgrown example to illustration;
- expose a technical relationship hidden by the current structure.

Do not reorganize reference around one reader project merely because that
would be appropriate for how-to documentation.