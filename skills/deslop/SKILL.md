---
name: deslop
description: >
  Detect, critique, and rewrite text to remove AI writing patterns — makes content sound human,
  specific, and credible. Use this skill whenever: writing any client-facing or published content
  from scratch; editing/polishing any draft that might sound "corporate AI"; asked to "make this
  sound more human", "remove AI patterns", "clean up AI text", "edit this", "improve this copy",
  "write a blog post / landing page / release note / announcement / marketing copy / product description".
  Also auto-apply when generating any text longer than ~3 sentences where quality matters.
  This skill should be consulted proactively — don't wait to be asked.
metadata:
  author: Ian Corvin
  version: "2.0"
---

# Deslop

Helps produce and edit text that reads like a specific, thoughtful human wrote it — not like a language model averaging across the internet.

## Core Principle

AI writing *regresses to the mean*: it replaces specific, unusual facts with generic, positive-sounding statements that could apply to anything. The fix is always the same: **be more specific, not more impressive-sounding**.

**Caveat before you start cutting:** perfect grammar, a formal/academic register, or prose that just feels "stiff" are *not* proof of AI on their own — plenty of skilled or non-native writers produce exactly that. Don't over-correct a text that's merely formal into something falsely casual. The patterns below are signs, not a checklist to mechanically strip from every sentence.

---

## Part 1: Red Flag Patterns (Detect & Remove)

### 1. AI Vocabulary Words

These words are statistically overrepresented in LLM output. One or two is fine. A cluster is a red flag. Remove or replace with simpler, more direct alternatives.

**Era 2023–2024 (GPT-4):**  
`additionally` (to start a sentence), `boasts`, `bolstered`, `crucial`, `delve`, `emphasizing`, `enduring`, `garner`, `intricate/intricacies`, `interplay`, `key` (as adjective), `landscape` (abstract), `meticulous/meticulously`, `pivotal`, `underscore` (verb), `tapestry` (abstract), `testament`, `valuable`, `vibrant`

**Era mid-2024–2025 (GPT-4o):**  
`align with`, `bolstered`, `crucial`, `emphasizing`, `enhance`, `enduring`, `fostering`, `highlighting`, `pivotal`, `showcasing`, `underscore`, `vibrant`

**Era mid-2025+ (GPT-5):**  
`emphasizing`, `enhance`, `highlighting`, `showcasing` — plus excessive attribution to named sources

**Model-specific:** Grok overuses superficially "scientific" words — `causal`, `empirical`, `correlate` — and, unlike GPT, kept overusing `underscore` well into 2026.

**Replacements:**
- `underscore` → show, prove, explain, make clear
- `delve` → look at, explore, get into
- `pivotal` → key, decisive, major, turning-point (or just cut it)
- `tapestry` → mix, combination, blend
- `leverage` → use
- `showcase` → show, display, demonstrate
- `foster` → build, grow, support
- `vibrant` → busy, active, lively (or just describe what makes it vibrant)

---

### 2. Significance Inflation

Attaching unsupported claims about importance, legacy, or broader impact.

**Patterns to cut:**
- "marking a pivotal moment in the evolution of..."
- "represents a significant shift toward..."
- "was part of a broader movement to..."
- "stands as a testament to..."
- "reflects broader trends in..."
- "symbolizing its ongoing/enduring legacy"
- "setting the stage for..."
- "underscores its importance/significance"
- "contributes to the rich tapestry of..."
- "indelible mark", "deeply rooted", "focal point"

**Fix:** Either state the specific fact that *demonstrates* significance, or cut the claim entirely.

> ❌ "The launch marked a pivotal moment in the evolution of documentation tooling."  
> ✅ "After the launch, customer onboarding time dropped from 3 weeks to 4 days."

---

### 3. Trailing Participle Analyses

Adding "-ing" phrases at the end of sentences to create an illusion of insight.

**Pattern:** `[factual statement], [present participle]-ing [vague significance].`

> ❌ "The station has 6 platforms, contributing to the socio-economic development of the region."  
> ✅ "The station has 6 platforms."

**Also watch for:** `ensuring`, `reflecting`, `highlighting`, `cultivating`, `fostering`, `encompassing` — especially when tacked onto otherwise neutral sentences.

**Related: Leading participle clauses.** Same problem, different end. "Recognizing the importance of X, companies must Y" / "Considering current trends, it is crucial to Z." Rewrite as two sentences or drop the clause.

---

### 4. Copula Avoidance ("serves as" disease)

LLMs replace "is/are" with more elaborate verb constructions to sound more sophisticated.

**Patterns:**
- "serves as a" → is a
- "stands as a" → is a  
- "marks the" → is the
- "represents a" → is a
- "boasts/features/offers" → has
- "ventured into politics as a candidate" → was a candidate

**Fix:** Use "is" or "are" when that's what you mean.

> ❌ "This feature serves as a solution for teams that need..."  
> ✅ "This feature solves a problem for teams that need..."

---

### 5. Vague Authority Attribution

Attributing claims to unnamed or inflated sources.

**Patterns:**
- "Industry reports suggest..."
- "Experts argue that..."
- "Observers have noted..."
- "Some critics argue..."
- "Research shows..." (with no citation)
- "It is widely recognized that..."

**Fix:** Name the specific source, or rephrase as your own claim, or cut it.

**Related — vague quantifiers.** The same weasel move applies to numbers, not just sources: "significantly", "many", "often", "typically", "generally" stand in for a number the writer either doesn't have or didn't bother finding.

> ❌ "Significantly improves load times for most requests."  
> ✅ "Cuts load times by 40% for the top 20% of requests."

---

### 6. Promotional / Travel-Guide Tone

Especially common in descriptions of products, companies, or places.

**Patterns:** `nestled`, `breathtaking`, `vibrant community`, `rich cultural heritage`, `groundbreaking`, `renowned`, `diverse array`, `natural beauty`, `in the heart of`

**Product-specific:** "commitment to excellence", "best-in-class", "seamlessly integrates", "powerful yet intuitive", "robust solution"

**Fix:** Describe what is actually there. Specifics > superlatives.

> ❌ "A vibrant platform that seamlessly integrates your workflow with powerful AI capabilities."  
> ✅ "A platform that syncs with GitHub and generates doc drafts from your commit messages."

---

### 7. Canned Emphasis on Notability / Media Coverage

Specific to bios, case studies, and PR-adjacent copy: instead of stating what someone did, AI hits the reader over the head with proof that they were *covered*.

**Patterns:** "featured in [Outlet], [Outlet], and other media outlets", "profiled in multiple independent outlets", "maintains an active social media presence", "has been mentioned in [X] coverage relating to..."

**Fix:** Name the one or two sources that actually matter and say what they said. Cut "and other media outlets" — it's padding, not evidence.

> ❌ "She has been featured in Forbes, TechCrunch, and other prominent media outlets."  
> ✅ "Forbes covered her Series A raise in March."

---

### 8. The Challenges Formula

Rigid structure that appears at the end of articles/sections:

> "Despite its [positive quality], X faces several challenges, including [...]. Despite these challenges, X continues to [vague optimism] / [future initiatives] could..."

**Fix:** Either cut the section, or make it concrete: name the specific challenge, what's been tried, what the actual status is.

---

### 9. Not-Just-X-But-Also-Y Parallelisms (and Negation-Inversion)

Constructions that sound "balanced and thoughtful" but say nothing:

- "Not only... but also..."
- "It's not just about X, it's about Y"
- "Not X, but Y"
- "This isn't just a tool. It's a transformation."
- "No X, no Y, just Z"

**Negation-inversion pattern:** sets up a strawman the reader never held, then "corrects" it for false drama. Especially suspicious when clustered 2+ times in a short piece.

**Reversed variant — "X rather than Y":** the same move flipped ("prioritizing consolidation of power rather than ideological purity"). Same fix applies.

> ❌ "This isn't just a feature. It's a paradigm shift. It's not about speed. It's about rethinking how teams collaborate."  
> ✅ "The feature cuts review time in half because it automates the three steps that used to be manual."

**Fix:** Either state X and Y as separate facts, or drop one of them. Occasional use is fine. Red flag when clustered or used to end a piece with a flourish.

---

### 10. Rule of Three (Overuse)

LLMs love tripling adjectives and noun phrases:
> "keynote sessions, panel discussions, and networking opportunities"  
> "global SEO professionals, marketing experts, and growth hackers"

Fine in moderation. Suspicious when every single sentence does it.

**Related — "from X to Y" false comprehensiveness:** "Our services range from strategic planning to implementation support" sounds thorough but says nothing concrete. Just list what's actually offered.

---

### 11. Elegant Variation (Synonym Spinning)

Avoiding repeating a word by cycling through synonyms: protagonist → key player → eponymous character → central figure.

**Fix:** Just repeat the word. Repetition is cleaner than a thesaurus parade.

---

### 12. Collaborative Communication Artifacts

Phrases that belong in a chat response, not in published content:

`I hope this helps`, `Of course!`, `Certainly!`, `Would you like...`, `is there anything else`, `let me know if`, `here is a [X] that`, `more detailed breakdown`

**Fix:** Cut entirely.

---

### 13. Knowledge Cutoff / Hedging Disclaimers

- "As of my last knowledge update..."
- "While specific details are limited in available sources..."
- "This person maintains a low profile..."
- "Based on available information..."

**Fix:** Either state what you know, or don't include it.

---

### 14. Em-Dash Overuse (Model-Specific Tell)

GPT-4o uses em-dashes roughly 10x more than GPT-3.5; Claude is more restrained; humans use them sparingly for real emphasis. Two or more em-dashes per paragraph is a strong tell — especially when unspaced and clustered.

> ❌ "The strategy — which involves multiple steps — requires planning — particularly around resources."  
> ✅ "The strategy has multiple steps. Resource planning matters most."

**Rule of thumb:** more than 1 em-dash per 200 words is suspicious. Mix em-dashes with commas, periods, and semicolons instead.

---

### 15. Uniform Rhythm (Burstiness Collapse)

Human writing is *bursty*: short punchy sentences mixed with long, clause-heavy ones. AI clusters around 12–18 words per sentence with low variance. Also: uniform paragraph heights (every paragraph ~3-4 sentences) reads as AI.

**Self-check:** Count sentence lengths in a paragraph. If they all sit within a 5-word band, rewrite at least one to be radically shorter (3-5 words) or longer (30+ words). Same for paragraph length: mix one-sentence paragraphs with longer ones.

> ❌ (all 12-15 word sentences) "Remote work changed everything. Teams spread across time zones. Communication became harder. Trust required new strategies. Leaders adapted quickly."  
> ✅ "Remote work broke everything — teams scattered, time zones fragmented the day. Leaders had to rebuild trust from scratch. It was messy."

**Don't confuse this with stop-start fragments (§16.1):** varying length on purpose is good; chopping *one* idea into three flat sentences because it's easier to generate is not.

---

### 16. Rhetorical Scaffolding

Sentences that announce the action instead of performing it:

- "Let's explore...", "Let's break this down", "Let's dive in", "Let's unpack"
- "Here's the thing..."
- "But here's where it gets interesting..."
- "Let me walk you through..."

Like someone clearing their throat before speaking. Great writers begin; mediocre ones announce.

> ❌ "Let's explore why this matters. Let's break down the key components."  
> ✅ "This matters because the cost model changed. The three key components are..."

**Fix:** Cut the announcement and start with the actual content.

#### 16.1 Stop-Start Fragments

A close cousin: splitting one dependent idea across several choppy sentences instead of writing it as one.

> ❌ "Previously this was manual. Now it's automatic. This saves time."  
> ✅ "What used to be manual is now automatic, saving time."

Short sentences used deliberately for emphasis (see §15) are fine. This is different: it's fragmenting a *single* thought because generating three short sentences is easier than building one properly subordinated one.

#### 16.2 Summary-Style Transitions

Opening a new paragraph by recapping the one before it, instead of moving forward.

> ❌ "With this setup complete, we can now look at..." / "Now that we've explored X, let's turn to Y."  
> ✅ "The catch is..." / "In practice, this means..."

#### 16.3 Cold-Open Paragraphs

A paragraph whose first sentence works as a standalone heading — no connective tissue to what came before. Carry the subject forward instead of starting fresh each time.

> ❌ (new paragraph, no lead-in) "Caching reduces latency significantly."  
> ✅ "Because the API call was the bottleneck, caching reduces latency here."

#### 16.4 Reused / Template Framing

A generic angle that could open any article on any topic, not something specific to this one.

> ❌ "The question most teams face is whether to build or buy."  
> ✅ (skip the throat-clearing, state the actual finding or fact first)

---

### 17. Opener Formulas

AI loves vague trend-setting intros:

- "In today's fast-paced world..."
- "In an era of [rapid change / digital transformation / AI disruption]..."
- "As we navigate the [modern / evolving / complex] landscape..."
- "Imagine a scenario where..."

**Fix:** Start with a concrete problem, a specific observation, a number, or a scene.

> ❌ "In today's fast-paced business environment, efficiency is more important than ever."  
> ✅ "Last quarter we lost 30% of trial users at the same onboarding step. Here's why."

---

### 18. Closer Formulas

AI can't resist wrapping up:

- "In conclusion...", "In summary...", "To sum up..."
- "As we move forward...", "Looking ahead...", "The future holds..."
- "The path ahead is clear..."
- Restating 3 key points verbatim in the final paragraph

**Fix:** End on a specific fact, a question left hanging, a surprising observation, or a concrete next step. Don't recap — readers just read it.

---

### 19. Nominalization Overuse

LLMs turn verbs into abstract nouns ("implement" → "implementation", "decide" → "decision-making", "analyze" → "analysis"). This creates dense, corporate-sounding text. Used at ~1.5–2x the rate of human writing.

> ❌ "The implementation of this strategy requires the establishment of clear governance and the acquisition of new resources."  
> ✅ "To roll out this strategy, we need governance and new resources."

**Self-check:** Count words ending in `-tion`, `-ment`, `-ance`, `-ity`, `-ness` in a paragraph. If more than 3-4 per paragraph, replace at least half with verbs.

---

### 20. Spec-Sheet Voice

Sentences that read like a line off a datasheet instead of something a person wrote: `provides`, `is configurable`, `is explicitly labeled`, `supports X functionality`.

> ❌ "The endpoint provides configurable retry logic and is explicitly labeled as idempotent."  
> ✅ "The endpoint retries automatically; you can tune how many times. Calling it twice is safe."

---

### 21. Personified Artifacts (technical writing)

Non-human things performing human, physical actions — common in product/API copy.

> ❌ "The browser hands the server a URL." / "The token holds the session."  
> ✅ "The browser sends the URL to the server." / "The session is stored in the token."

**Fix:** Give the object the verb that actually describes what it does, not a borrowed human action.

---

### 22. Formatting Overload

LLMs over-format because markdown structure is easy to generate:

- **Bold-inside-prose for fake emphasis** ("the **most important** thing is..."). More than 1-2 bolds per section = tell.
- **Bold-lead-colon pattern:** "**Key insight:** ..." repeated every paragraph.
- **Excessive H2/H3 headers** where prose would flow.
- **Numbered lists for flowing thoughts** ("Here are 5 reasons: 1. Cost. 2. Speed. 3. Quality...") when a sentence would do.
- **Rigid scaffolding:** Overview → Key Points → Challenges → Conclusion.
- **Emoji clusters** (🔑🎯💡) as bullet markers in serious content.

**Fix:** Prose by default. Use lists only for genuinely list-like content (comparisons, instructions, features). Use headers only for navigation in long pieces. Bold sparingly, for one key phrase per section at most.

---

### 23. Self-Answered Rhetorical Questions

AI asks a question the reader wasn't asking, then answers it. Repeatedly.

> ❌ "What does this mean for your team? It means you need to rethink communication. Why is that important? Because remote work changed everything."  
> ✅ "Remote work changed how teams communicate. Async beat sync, not because anyone planned it, but because timezones won."

**Fix:** If you pose a question, either leave it hanging for the reader, or answer with evidence (not restatement). One rhetorical question per piece is usually enough.

---

### 24. Over-Hedging Clusters

Stacking cautious qualifiers: "arguably", "potentially", "it could be said", "it's worth noting", "one could argue", "may", "might", "could potentially", "perhaps".

> ❌ "This approach could potentially unlock new opportunities, arguably transforming how teams might leverage existing resources."  
> ✅ "This approach cut delivery time by 40% on two projects. It might not scale — but so far it works."

**Fix:** Commit. If you're uncertain, say so directly once. Don't blanket the whole text with maybes. (Note: one hedge in isolation is normal human writing — see Part 2, §13 — this is about *stacking*, not using any hedge at all.)

---

## Part 2: Positive Principles (What Human Writing Does Instead)

1. **Specific > Generic.** "Our conversion rate doubled" beats "significant improvement was achieved."

2. **Show, don't infer significance.** Let facts speak; don't tell readers what to conclude.

3. **Use "is/are" freely.** It's direct. It's clear. It's fine.

4. **Repeat words.** "The product → it → the tool → this solution" is AI. "The product → the product" is human.

5. **Cut trailing analysis.** If a sentence ends with a present participle clause that explains why the previous fact matters, cut that clause.

6. **Name sources or cut attribution.** "Experts say" = AI filler. Name the expert, or say it yourself.

7. **One structural tell to break:** avoid the rigid "background → current state → challenges → future outlook" outline. Real writing has narrative, not sections.

8. **Vary sentence length aggressively.** Short sentences. Then a medium one that adds context. Then a longer one that complicates the picture or adds a caveat, because that's how ideas actually develop — not in perfectly parallel triplets. Include at least one sentence under 6 words and one over 25 words per page.

9. **Prefer verbs over abstract nouns.** "We decided" beats "decision-making was undertaken". Verbs carry energy; nominalizations drain it.

10. **Don't announce — just do.** Cut "Let's look at...", "Here's the thing...", "Now let me explain...". The reader is already reading.

11. **Don't recap at the end.** End on something the reader hasn't read yet — a specific fact, a surprise, a question, a next action.

12. **Format for readers, not for models.** Prose by default. Bold only for one phrase per section. Lists only for list-like content.

13. **Use plain words over their stiff synonyms — freely.** "Wrote" not "authored". "Used" not "utilized". "Moved" not "relocated". "Tried" not "attempted". "Died" not "passed away". AI systematically avoids the plain version in favor of the fancier one; using the plain word is one of the more reliable ways to *not* sound like AI, not a dumbing-down.

14. **Make definitive claims when they're true.** "Was the first", "is the only", "one of the best" — AI hedges away from these even when accurate, because it's trained to avoid overclaiming. If it's true and you can back it up, just say it.

15. **Don't reflexively strip "unnecessary" wordiness.** Phrases like "in order to", "as a result of", "the fact that", "a part of" are actually *more* common in human writing than AI output, not less. If a passage feels over-processed, adding a little natural wordiness back can help more than more cutting.

16. **Simple "there is / it has" constructions are fine.** AI tends to dress these up into something more elaborate. You don't need to.

---

## Part 3: Editing Protocol

When asked to clean up or rewrite AI-sounding text, proceed in this order:

1. **Identify clusters** of red-flag vocabulary (Part 1, §1)
2. **Find trailing/leading participle phrases** (§3) and cut them
3. **Restore copulas** — replace "serves as", "stands as" with "is" (§4)
4. **Remove significance inflation** (§2) unless specific evidence is provided
5. **Flatten promotional tone** (§6) — replace adjectives with facts
6. **Check attribution and quantifiers** (§5) — name sources, cite numbers, or cut
7. **Count em-dashes** (§14) — reduce to 1 per 200 words max
8. **Check rhythm** (§15) — inject sentence-length variation and paragraph-length variation, but don't confuse this with stop-start fragmenting (§16.1)
9. **Cut scaffolding** (§16) — "Let's..." preambles, announcements, rhetorical throat-clearing, summary-style transitions (§16.2), cold-opens (§16.3)
10. **Kill opener/closer formulas** (§17, §18) — start specific, end specific
11. **Reduce nominalizations** (§19) — turn noun phrases back into verbs
12. **Fix spec-sheet voice and personified artifacts** (§20, §21) — mostly relevant for technical/product copy
13. **Deformat** (§22) — less bold, fewer bullets, fewer headers unless they earn it
14. **Restore plain words and definitive claims** (Part 2, §13-14) — don't over-launder simple language back into something fancier
15. **Passive voice check:** append "by monkeys" to the sentence. If it still parses, it's passive — rewrite active where it matters.
16. **Second-read test:** read each sentence once at speaking pace. If you have to re-read it to find the subject, the action, and the consequence, cut the metaphor verbs or the pronouns reaching back too many sentences.
17. **Read aloud test** — if a sentence sounds like it was written for a brochure, rewrite it

When generating new content, apply Part 2 principles from the start rather than editing after.

---

## Part 4: Context-Specific Notes

### Product / SaaS copy
Most common trap: "powerful, intuitive, seamless" trinity. Replace with one specific capability + one specific outcome.

### Release notes / changelogs  
Most common trap: significance inflation ("marking a major milestone"). Just describe what changed and what it enables. Watch for spec-sheet voice (§20) and personified artifacts (§21) here specifically — release notes describe systems, and it's easy to slip into either.

### Blog posts / thought leadership
Most common traps: challenges formula, significance trailing phrases, vague attribution. Use named examples, specific numbers, first-person opinions.

### Marketing landing pages
Most common traps: promotional tone, copula avoidance. Write like you're explaining to a smart friend, not pitching to a committee.

### Telegram / short social posts
Most common traps: opener formulas, self-answered rhetorical questions, excessive emoji/bold. A TG post should sound like a voice message you typed out, not a mini-blog-article with headers.

### Bios / case studies / PR-adjacent copy
Most common trap: canned emphasis on notability (§7) — listing outlets instead of stating facts. Name the one thing that matters; cut "and other media outlets".

---

## Quick Reference: Before/After

| AI version | Human version |
|---|---|
| "serves as a critical component" | "is essential" or "is the key piece" |
| "highlights the enduring significance" | (cut) |
| "contributing to socio-economic development" | (cut, or cite specific data) |
| "vibrant ecosystem of tools" | "a growing set of tools" |
| "delve into the intricacies" | "look at how X works" |
| "fosters collaboration" | "helps teams work together" |
| "leverage your existing workflow" | "use your existing workflow" |
| "Not just X, but also Y" | state X and Y as separate facts |
| "Despite its challenges, X remains..." | state the challenge concretely |
| "Experts argue that..." | "According to [Name]..." or cut |
| "Let's break this down..." | (cut — just start) |
| "In today's fast-paced world..." | start with a specific fact |
| "In conclusion..." | (cut — end on substance) |
| "The implementation of X requires..." | "To do X, you need..." |
| "This isn't just a tool. It's a revolution." | "This tool cut onboarding from 3 weeks to 4 days." |
| "featured in Forbes, TechCrunch, and other outlets" | "Forbes covered the Series A raise in March." |
| "provides configurable retry logic" | "retries automatically; you can tune how many times" |
| "the token holds the session" | "the session is stored in the token" |
| "authored" / "utilized" / "attempted" | "wrote" / "used" / "tried" |
| "With this setup complete, we can now..." | "In practice..." / "The catch is..." |
