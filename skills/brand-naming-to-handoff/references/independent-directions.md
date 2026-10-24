# Independent direction authors

## Responsibilities and isolation

The coordinator establishes the brief, preserves constraints, and makes comparison fair. Each author independently discovers a visual idea. Do not allocate predetermined territories such as moon imagery to one author and marble to another, or write everyone's prompts centrally. Convergence is possible; detect it after independent discovery and address it in a separate round.

Usually start with 2–3 authors, subject to the request, available slots, and cost. Do not create user-owned chats as a substitute for subagents. Give each author an isolated context and output folder, such as `directions/a/`, so they do not read or overwrite sibling work. Avoid passing the complete conversation when it reveals other concepts. If the API forces inherited history, disclose that limitation or use fresh sessions where available.

## Assignment contract

Build a concrete assignment from these fields; do not return an unfilled template:

- Product, audience, primary job, and verified capabilities.
- The fixed name or agreed candidate; established constraints and what remains open.
- Intended perception, public promises, and prohibited claims.
- Shared English customer-facing text in sentence case.
- Surfaces, dimensions, level of finish, available tools, and output folder.
- Task: independently discover a compelling visual territory, inspect real references, and write an exact prompt. Do not read sibling folders. Return a concept card before rendering; realize the concept after the coordinator checks differentiation.

Pass actual constraints only. Do not add Daymoon's moon imagery, light palette, or restraint to an unrelated brief.

## Return contract

1. A direction name and a one-sentence idea.
2. Why it fits this product and its main tradeoff.
3. Inspected references: link or file, what was examined, and which properties inform the concept. Mark inaccessible sources. A link found but not opened is not an inspected reference.
4. Composition, typographic character, palette, imagery/materials, mark, and behavior in product UI. These are proposals, not finalized tokens.
5. The author's exact prompt, negative constraints, and acceptance criteria.
6. After realization: artifacts, generation metadata, and an inspection note including discrepancies between intent and result.

## Check differentiation

Compare metaphor, visual grammar, composition, typography, materials, and relationship to the product. Could the direction be recognized with the name and colors hidden? Treat that as a heuristic, not a formal test or a requirement to remove branding from real mockups.

If cards duplicate one another, tell an author: "The concept is insufficiently differentiated in composition and visual language. Independently explore another territory from the product brief while preserving the established constraints." Do not reveal the sibling prompt or prescribe the answer. Start with one additional round. If convergence persists, disclose it rather than calling the results fully distinct; expand exploration further when the task requires it.

Continue with the same authors for realization without revealing sibling results. If image generation has a global concurrency limit, coordinate a rendering queue: sequential rendering does not negate independent concept discovery. Assemble the comparison board only after results return.

## When subagents are unavailable

Do not simulate messages from nonexistent agents. Work in separate passes, committing each concept card and prompt before the next, avoiding template reuse, and stating that one agent is working without true context isolation. Prepare assignments for independent fresh sessions if useful and supported. This fallback is not equivalent to independent discovery.
