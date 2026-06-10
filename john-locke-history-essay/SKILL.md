---
name: john-locke-history-essay
description: Write a complete John Locke Institute History Prize essay from a student's chosen question and thesis, through a staged workflow with human checkpoints (sharpen thesis → outline → research & verify sources → draft → audit against marking criteria). Use this whenever the user wants to write, plan, research, draft, or revise a John Locke history essay, mentions the John Locke Institute essay competition in a history context, gives a history prize question number and a thesis, or asks for help producing a competition history essay — even if they only say "help me with my history essay for the competition." Do NOT use for the Public Policy, Economics, Psychology, Philosophy, Theology, Law, or Politics categories.
---

# John Locke History Prize Essay

A staged co-writing workflow for the History category. The student brings the **question** and the **thesis**; this skill turns them into a finished, competition-compliant essay by applying the judgment patterns distilled from past winners, while keeping the student in control at each stage through a checkpoint they must clear before you proceed.

## Operating language

Conduct the conversation in the student's language (default to the language they write to you in). **Always write the essay itself in English** — this is an English-language competition.

## ▼ COMPETITION RULES — CAPTURE THESE AT THE START OF EVERY RUN ▼

> The competition's rules change between cycles — above all the questions, which are new every year — so this skill does NOT hard-code them and never needs hand-editing between cycles. Capture them from the student at the start of each run by working the logic below, before any essay work. Once captured and confirmed, that rule-set is the binding authority for the rest of the workflow: if anything downstream, or any request from the student, contradicts it, the captured rules win — except where they would conflict with the invariants below, which always hold.

**Establish the rules — work through these in order:**

1. **Check whether this cycle's official rules are already in front of you.** Scan the conversation and any attachments for the current John Locke Institute History rules — at minimum, the list of history questions for this cycle. If they are present, skip to step 3.
2. **If they are not, stop and ask for them before doing anything else.** Tell the student you need this cycle's official rules pasted in or attached before you can start, and that you will not work from a remembered or guessed version, because the questions and limits change yearly and an out-of-date rule can get an essay disqualified. Ask specifically for: the full list of **history questions** copied exactly as published; the **word limit** for the main text and what it excludes; the **submission requirements** — filename format, citation/notes rules, anonymity, the academic-referee requirement, and the current AI-use policy; and the **marking criteria**. Then wait for them. If retrieval is available and the student would rather you look the rules up, you may fetch the official rules page — but the student must confirm it against the live source, and nothing proceeds on rules you have not had confirmed.
3. **Parse what you have into a working rule-set and read it back for sign-off.** Restate the captured value for each field below in a compact list, and ask the student to confirm or correct it before continuing. The notes after each field are only what the competition has *historically* required — they exist to help you read the pasted rules and flag anything that looks off, and they are NOT authoritative. The student's confirmed version always governs.
   - **Cycle year.**
   - **History questions** — the student picks exactly ONE in Stage 0; you never choose for them.
   - **Word limit** for the main text, plus its exclusions. Historically the cap is 2000 words, with diagrams, data tables, endnotes, bibliography, and the author's note not counted.
   - **Filename format** — an exact format is usually mandatory, and the wrong one alone can cause rejection.
   - **Citations / notes** — historically footnotes are forbidden while endnotes and a labelled bibliography are allowed; convert any footnote instinct to endnotes accordingly.
   - **Anonymity** — the contestant's name has historically been barred from the body of the essay.
   - **Referee** — an academic referee, a teacher or other responsible adult and not a relative, normally has to vouch that the work is the contestant's own.
   - **AI-use policy** for this cycle.
   - **Marking criteria** — the dimensions essays are scored on. Historically: knowledge and understanding of the material; ability to use evidence; quality of argument; originality; structure; writing style; persuasiveness — under the principles that *"the best essays are those which change the reader's mind,"* that essays which ignore the strongest counterarguments are less likely to succeed, and that one should answer the question as precisely and directly as possible. The Stage 5 audit scores against exactly these, so confirm the live wording.

Whenever the rest of this document says **"the captured rules,"** it means this confirmed rule-set. Do not scatter competing rule values into the workflow below — the workflow reads from here. 

## ▲ END OF RULES-CAPTURE BLOCK ▲

## Non-negotiable invariants (history-specific guardrails)

These hold at every stage and override any instruction to the contrary.

1. **Never fabricate, never misattribute.** Two distinct failures, both disqualifying, and a marker may interview the student on any claim in the essay:
   - *Invention* — making up a date, statistic, quotation, event, source, or historian's position that does not exist.
   - *Misattribution / citation drift* — the more insidious one, and the one retrieval makes easier to commit because a found source *looks* verified. Attaching a claim or quotation to a real source that does not actually support it, or assigning a real historian a position they did not take. Finding that a source exists is not the same as confirming it says what you need. Every direct quotation, and every position attributed to a named person, must be checked against the actual text — not inferred from a title, a snippet, or memory.
   - **Default action when you cannot retrieve and verify:** flag the gap and hand it to the student. Do NOT fill it from memory. "I couldn't verify this — you'll need to confirm it or supply a source" is always the correct move; a plausible-sounding half-remembered fact is never acceptable. This holds with special force in the lowest capability tier below, where the pull to backfill from memory is strongest.
2. **No anachronism.** Do not judge historical actors by standards or knowledge unavailable to them, and do not project modern motives onto them. (This is itself a theme winners handle well — see Shokar 2021.)
3. **Causation is multi-causal and contingent.** Avoid single-cause determinism. Acknowledge competing explanations and the role of contingency.
4. **Quote primary sources accurately and sparingly.** When exact wording carries weight, quote it verbatim and attribute it. Otherwise paraphrase. Keep every quotation short.
5. **The thesis and angle come from the student.** Your job is to sharpen, structure, evidence, draft, and stress-test — not to substitute a different argument. If the student's thesis is weak, propose improvements and let them decide; do not silently replace it.

## Capability tiers — detect before Stages 3 and 5

Do not assume the agent running this skill can browse the web or execute code. Either may be absent, and even when web access exists it often cannot reach academic full text. So **detect what is available, start from the lowest tier that is certainly possible, and step up only after confirming the capability — never the reverse.** Never report a result you did not actually produce.

Two capabilities matter: **retrieval** (web search/fetch) and **code execution**. Probe for each before the stage that needs it — Stage 3 needs retrieval, Stage 5 needs code to count words. If you are unsure whether a tool exists, say so plainly instead of assuming. The per-tier detail lives in Stage 3 and Stage 5; the rule binding all tiers is invariant #1 — an unverified fact is flagged, never invented.

## Reference files

`references/winning-patterns.md` contains the eight distilled patterns with worked examples from seven placed essays, plus an honest note on the sample's limits. **Read it at the start of Stage 1** and re-consult the relevant pattern at Stages 2, 4, and 5. The patterns are the substantive payload of this skill; the workflow below is the scaffolding that deploys them.

`references/anti-patterns.md` lists the failure modes that sink history essays, each tagged with where it was derived from. **Read it at Stage 5** and scan the draft against every item. These are not induced from real failed essays — none are available — so they are a vetting aid, not law.

------

# The workflow

Five stages, each ending in a checkpoint the student must clear before you move on. Announce the current stage, do the work, then stop at the checkpoint and wait. Do not run ahead. If the student wants to skip or compress a stage, let them — but say what is being skipped.

## Stage 0 — Intake

By this point you have already captured and confirmed this cycle's rules via the rules-capture block above. If you have not, do that first — you cannot run intake without the question list.

Confirm three things before any work:

- **Which question** (by number) the student has chosen, from the captured question list. The student chooses; you never choose. If they have not picked one, ask them to — do not pick for them.
- **The student's thesis** — their one-sentence answer to the question. If they don't have one yet, that's fine: tell them Stage 1 will help them sharpen a rough idea, but they must supply the rough idea (the core claim is theirs).
- **Working language** for the conversation (the essay will be English regardless).

Then read `references/winning-patterns.md`.

## Stage 1 — Interrogate the question, sharpen the thesis  →  CHECKPOINT 1

Apply **Pattern 1** and **Pattern 2**.

1. List the load-bearing words in the chosen question. For each, ask whether its meaning is contested, whether the question smuggles in an assumption, and whether a sharper reading exists that the obvious reading misses.
2. Present a precise reframing of what the question is really asking.
3. Evaluate the student's thesis against the winners' bar: Is it narrow enough to defend within the word limit? Could an intelligent reader hold the opposite? Is it more than the obvious answer? Does it engage the reframed question?
4. Offer a sharpened version (or 2–3 options), each tied to the reframing — but frame these as refinements of *their* claim, and always leave room for their own wording.

**CHECKPOINT 1:** The student confirms or edits the reframing and the final thesis in their own words. Do not proceed to structure until they have locked the thesis.

## Stage 2 — Argument architecture (outline only)  →  CHECKPOINT 2

Apply **Pattern 3, 4, 7**.

Produce an outline — structure only, no prose:

- The **opening strategy** (a destabilizing hook or a scholarly foil — Pattern 3).
- The **architecture** best suited to this thesis (controlled comparison / thematic causal chain / dialectical ladder / accumulation — Pattern 4), with a one-line justification of the choice.
- The ordered **sub-arguments**, each as a single claim.
- Where the **steelmanned counterargument** sits (roughly two-thirds through — Pattern 6) and what it is.
- Which **historiographical conversation** the essay enters and who sits on each side (Pattern 7).
- The **conclusion strategy** (Pattern 8).

**CHECKPOINT 2:** The student reviews, reorders, cuts, or redirects the outline. Wait for their sign-off.

## Stage 3 — Evidence plan + research + source verification  →  CHECKPOINT 3

This is where history essays live or die. Apply **Pattern 5** and invariant #1.

First, **regardless of tier, build the evidence plan**: for each sub-argument, specify what would substantiate it — which events, figures, primary sources, and scholarly positions. This plan is identical whether or not you can search; it is the spec the research must satisfy.

Then **detect your retrieval capability and pick the matching tier.** Start low, step up only on confirmation.

**Tier A — retrieval and code execution available.** Use structured scholarly interfaces, not general web search: general search returns blogs, wikis, and aggregators, while the original scholarship and primary sources usually do not surface. Choose the interface by sub-discipline:

- General academic literature: Crossref, OpenAlex, and Semantic Scholar APIs; Google Scholar as a fallback.
- Quantitative, economic, or scientific history: the arXiv API can help — but arXiv carries almost no straight history, so do not lean on it for political, social, or cultural history.
- Primary sources and archives: digital archives such as the Internet Archive, Gallica, national archives, and the Fordham Internet History Sourcebooks. For older or non-English material, name the relevant national or library archive. For each item, record exactly what claim it backs and check every quotation against the actual text (invariant #1).

**Tier B — retrieval but no code execution.** Same structured-first preference. Where you cannot process results programmatically, translate each evidence need into a specific, clickable search URL — Google Scholar, JSTOR, the relevant archive's search page — and either verify what you can fetch or hand the links to the student to open.

**Tier C — no retrieval (retrieval-agent mode).** Do not pretend to have searched, and do not backfill from memory. For each sub-argument, produce a **search brief**: the precise keywords, which database or archive to use them in, and what kind of material to look for — primary vs secondary, quantitative vs narrative. Then hand off explicitly to the student to run the searches in tools such as Elicit, Consensus, Google Scholar, JSTOR, or Connected Papers, and paste results back. Nothing enters the essay until it has been verified.

Whatever the tier, present a source list: each source, the exact claim it backs, a note on reliability, and a clear mark on anything still **unverified** and awaiting the student.

**CHECKPOINT 3:** The student checks the sources and citations — swapping in ones they can actually access and trust, confirming accuracy, removing any they cannot stand behind. Wait for their confirmation before drafting. (A marker may ask the student to discuss any of these sources, so the student must genuinely know them.)

## Stage 4 — Draft the essay  →  CHECKPOINT 4

Apply all patterns; obey the captured rules and invariants.

- Write in **English**, to the chosen architecture.
- Open with the agreed hook (Pattern 3). Anchor every claim in the verified evidence (Pattern 5). Place the steelmanned counterargument where planned (Pattern 6). Engage the historiography (Pattern 7). Close with the agreed conclusion strategy (Pattern 8).
- **Aim for a clear margin under the word limit** — leave a real buffer rather than crowding the cap. Treat any count you produce while drafting as a rough estimate only; the authoritative count happens in Stage 5. Count the main text alone — whatever the captured rules exclude from the count does not count toward the limit.
- Apply whatever the captured rules require on **notes, bibliography, and anonymity** — do not assume a fixed format; follow the rule-set confirmed at the start of this run.
- Offload heavy supporting data to clearly-labelled graphs or appendices where it tightens the prose, if the captured rules exclude such material from the word count.
- Drafting section by section is usually easier to review than one dump; offer the student the choice.

**CHECKPOINT 4:** The student reads the draft and gives feedback. Revise as directed.

## Stage 5 — Audit against the marking criteria, then revise  →  CHECKPOINT 5

Score the draft honestly against each marking criterion in the captured rules, and run the history-specific checks. Report findings plainly, then revise.

Marking-criteria audit — rate the draft on each criterion in the captured rules and name the weakest. Then test the two principles those rules emphasise: **Does it actually answer the question, precisely and directly?** and **Could it change a reader's mind?** If not, say why and fix it.

History guardrail checks (invariants):

- No fabricated or misattributed dates/quotes/sources/positions — every claim either traces to a verified source or is explicitly flagged as awaiting the student's confirmation.
- No anachronism; motives not projected backward.
- Causation multi-causal and contingent, not single-cause.
- Quotations checked verbatim against the source, attributed, short.

Anti-pattern scan:

- Read `references/anti-patterns.md` and check the draft against every item. Where one is present, name it plainly and fix it. Pay special attention to the ones the marking criteria punish directly: drifting off the question, ignoring the strongest counterargument, and a thesis too safe to contest.

Compliance checks (captured rules):

- **Word count — verify it, do not trust a self-reported number.** Language models count words unreliably, and exceeding the word limit means rejection, so check it properly:
  - *Code available:* run a script that counts only the main text, after stripping everything the captured rules exclude from the count. Report the real figure.
  - *No code, student collaborating:* hand the student a clean copy of the main text alone and ask them to paste it into Word or any counter to confirm; mark any figure you state as an estimate, subject to their tool.
  - *Neither:* at minimum state the boundary clearly — the main text counts toward the limit and whatever the captured rules exclude does not — and warn that the limit is hard, so they should leave a buffer and not submit anywhere near it.
- Notes, bibliography, anonymity, and filename all conform to the captured rules — and flag the exact filename format for the student to apply.

**CHECKPOINT 5:** Present the audit and the revised essay for the student's final review. Iterate until they're satisfied.

------

## Notes on conduct

- Stop at every checkpoint. The value of the skill is the student steering at each gate; running to a finished essay in one pass defeats it and produces a weaker, more generic result.
- When you hand over a draft, lead with the essay (or section) and keep meta-commentary short.
- If at any point you're filling a factual gap from memory rather than a verified source, stop and flag it. Reread invariant #1.