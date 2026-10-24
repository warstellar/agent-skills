# Daymoon: project decisions and constraints

Apply this reference only to the AI-readiness checker for documentation. Do not carry its style or business context into unrelated brands. This records available evidence as of 24 October 2026; it does not verify the current product implementation.

## Sources and recovery limits

Primary conversation: "Name the checker" (translated title), conversation ID `6ad751c8-24a4-83ed-91b3-488f3a8b99b6`. Reading it with `read_thread`, `turnLimit=10`, returned only five recent turns, `hasMore=false`, and no cursor. Earlier naming exploration, original images, and two assistant responses represented by `chatgpt-content-reference` placeholders were unavailable. Do not invent the complete candidate list, prompts, fonts, colors, or image details.

Evidence anchors:

- `f59137dd-3275-44ab-bc9f-af349fd7a5f5`: the user objected that the branding looked identical (translated paraphrase). This establishes a differentiation failure, not the appearance of inaccessible images.
- `fac295e2-eff1-4c4b-ae93-1c8c5646eddf`: the user preferred Daymoon and requested directions/prompts followed by subagents or two passes. This does not prove later image generation succeeded.
- `9a61a971-4de3-4223-940b-3be5bbc73816`: request for an opinion; assistant response `cf303f24-389b-4d5b-8e6b-08f4870a9d33` recommends Daymoon and practical UI/reporting informed by Marble.
- `4e91e29c-dbb9-4ccf-8860-5b90e816608e`: request for a handoff; response `997476c8-338d-4dd6-96e6-44f38478fce0` contains a complete brand handoff draft. Unless noted otherwise, details below come from this draft. Requesting a handoff does not approve every detail in it.
- `5f6c2f8a-4ec4-4400-8dfc-7b38917ad4d8`: request to turn the conversation into a skill; the assistant response was not recoverable.
- Follow-up requirements on 24 October: Russian discussion, English customer-facing copy in sentence case; general process separate from Daymoon. Each variant needs an independent subagent that discovers its own direction from the common brief. This supersedes the earlier idea of centrally writing all directions and prompts. The latest correction requires all skill instructions, references, and metadata to be English and maintained in the agent-skills project.

## Working name decision

Daymoon is the preferred working brand, supported by explicit user preference and the assistant's recommendation. Marble remains the backup in the draft. Do not restart naming without a new request.

Reasons discussed: a memorable independent identity; daytime sky, moon, light, air, perspective; potential for a landing page, avatar, and Product Hunt. These are judgments, not user-test results or proof of legal availability. Domain, trademark, and registration checks are absent from the recovered record.

## Product and business context from the draft

- Category: AI readiness checker for documentation.
- Scenarios: check one documentation URL, compare two URLs, identify changes, and provide practical signals for stakeholder discussions.
- Emphasis: understandable before/after comparison and explainable results. These capabilities are brief statements; implementation and analytical accuracy were not verified here.
- Audience: documentation teams, technical writers, and docs leads; also product, support, success, and managers.
- Strategic constraint in the draft: an independent public product in v1 without obvious ClickHelp branding. Do not mention Reader UI in customer-facing copy or UI. The internal business role supports AI-readiness discussions and migration to the new Reader UI; keep it out of public promises.
- Meaningful findings and practical suggestions matter more than a vanity score. One score does not prove answer quality across every AI system.

## Verbal direction: working copy

Descriptor: **AI readiness checker for documentation**.

Draft lead message: **Compare two URLs and see what improved.** For neutral comparison, **Compare two URLs and see what changed.** may be proposed as a new edit, not represented as a past decision. Unchanged or worse results must remain visible.

Other draft suggestions, not final approvals: **Clarity for documentation in the age of AI**, **Clearer docs. Brighter answers.**, **Make your documentation AI ready.**

Voice: calm, direct, useful, grounded, slightly warm. Short copy, sentence case, no hype or inflated claims. CTA candidates: **Check your docs**, **Compare docs**, **Run a check**, **See what changed**. Avoid **Unlock AI excellence**, **Supercharge your knowledge base**, and **Revolutionize your docs**.

## Visual territory from the draft

Working territory: air, daylight, moon, openness, calm perspective. Light, spacious, quiet, architectural. Marketing can feel airy; product UI and reports should remain structured and practical. This is the assistant's recommendation in the comparison with Marble, not a verified finished design.

Proposed elements: pale sky blue, warm off-white/cream, muted navy, mist blue, restrained peach/dawn accents; soft light, an open horizon, arches/curves, and generous whitespace. These are directions, not approved hex values or proportions.

Mark proposal: a simple moon/eclipse/overlap symbol with a clean wordmark, legible as a small icon. Typography proposal: a clear modern UI sans, optionally an editorial display face for brand moments. Specific fonts, logo masters, and production files are not established.

Draft exclusions: a childish mascot brand, generic AI blue-gradient styling, cyberpunk, robots, overloaded space/star imagery, astrology, heavy 3D SaaS blobs, and excessive decoration. These exclusions apply to Daymoon, not all brands.

## Proposed next handoff

The draft proposes focused logo exploration, wordmark and symbol, app icon, palette, typography, and a mini brand sheet; then a landing hero, Product Hunt thumbnail, OG card, result preview, and comparison-flow mockup. Product surfaces include home, comparison form, results, a shareable snippet, and relevant loading/empty states. This is a plan, not evidence that files exist or a mandatory scope for every iteration.

## Separate historical image task

A historical note from 23 October concerns later image work in `ai-ready-docs-checker`, not the five recovered turns. It records a task-specific requirement for calm open sky in the left 55%, architecture on the right, no text/UI, and sidecar metadata with the exact prompt, tool, and dimensions. The recorded outcome was partial: the moons appeared closer to half-lit than the requested gibbous phase.

For continuation of that same image task, inspect negative space and moon phase separately. Do not turn 55%, gibbous moons, or right-side architecture into general Daymoon rules. Provenance: session `01a16a0b-2eb0-79d1-947d-8e13b19ffcba`, historical image-generation summary dated 23 October 2026. Files, sizes, and appearance were not reverified for this skill and may be outdated. Inspect current source assets before reuse. Images are not bundled or claimed to have been inspected here.
