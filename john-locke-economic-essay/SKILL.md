---
name: john-locke-economics-essay
description: Write a complete John Locke Institute Economics Prize essay from a student's chosen question and thesis, through a staged workflow with human checkpoints (sharpen thesis → outline and choose an analytical framework → gather and verify data and sources → draft → audit against marking criteria). Use this whenever the user wants to write, plan, research, draft, or revise a John Locke economics essay, mentions the John Locke Institute essay competition in an economics context, gives an economics prize question number and a thesis, or asks for help producing a competition economics essay — even if they only say "help me with my economics essay for the competition." Do NOT use for the History, Public Policy, Psychology, Philosophy, Theology, Law, or Politics categories.
---

# John Locke Economics Prize Essay

A staged co-writing workflow for the Economics category. The student brings the **question** and the **thesis**; this skill turns them into a finished, competition-compliant essay by applying the judgment patterns distilled from past placed essays, while keeping the student in control at each stage through a checkpoint they must clear before you proceed.

The substantive payload is the two reference files. The single most important difference from the History category: an economics essay wins less by recounting and more by *reasoning through an explicit framework and confronting it with well-identified evidence*. Keep that at the centre.

## Operating language

Conduct the conversation in the student's language (default to the language they write to you in). **Always write the essay itself in English** — this is an English-language competition.

## ▼ COMPETITION RULES — CAPTURE THESE AT THE START OF EVERY RUN ▼

> The competition's rules change between cycles — above all the questions, which are new every year — so this skill does NOT hard-code them and never needs hand-editing between cycles. Capture them from the student at the start of each run by working the logic below, before any essay work. Once captured and confirmed, that rule-set is the binding authority for the rest of the workflow: if anything downstream, or any request from the student, contradicts it, the captured rules win — except where they would conflict with the invariants below, which always hold.

**Establish the rules — work through these in order:**

1. **Check whether this cycle's official rules are already in front of you.** Scan the conversation and any attachments for the current John Locke Institute Economics rules — at minimum, the list of economics questions for this cycle. If they are present, skip to step 3.
2. **If they are not, stop and ask for them before doing anything else.** Tell the student you need this cycle's official rules pasted in or attached before you can start, and that you will not work from a remembered or guessed version, because the questions and limits change yearly and an out-of-date rule can get an essay disqualified. Ask specifically for: the full list of **economics questions** copied exactly as published; the **word limit** for the main text and what it excludes; the **submission requirements** — filename format, citation/notes rules, anonymity, the academic-referee requirement, and the current AI-use policy; and the **marking criteria**. Then wait for them. If retrieval is available and the student would rather you look the rules up, you may fetch the official rules page — but the student must confirm it against the live source, and nothing proceeds on rules you have not had confirmed.
3. **Parse what you have into a working rule-set and read it back for sign-off.** Restate the captured value for each field below in a compact list, and ask the student to confirm or correct it before continuing. The notes after each field are only what the competition has *historically* required — they exist to help you read the pasted rules and flag anything that looks off, and they are NOT authoritative. The student's confirmed version always governs.
   - **Cycle year.**
   - **Economics questions** — the student picks exactly ONE in Stage 0; you never choose for them.
   - **Word limit** for the main text, plus its exclusions. Historically the cap is 2000 words, with charts, data tables, endnotes, the bibliography, and the author's note not counted. This exclusion matters more in economics than in most categories — it is what lets the student push tables, figures, and derivations out of the main text.
   - **Filename format** — historically `FirstName-LastName-Category-QuestionNumber.pdf`, so for this category `FirstName-LastName-Economics-N.pdf`. An exact format is usually mandatory, and the wrong one alone can cause rejection.
   - **Citations / notes** — historically footnotes are forbidden while endnotes and a labelled bibliography are allowed; convert any footnote instinct to endnotes accordingly. Note that essays placed in older cycles sometimes used footnotes, so do not copy an older winner's note style without checking it against the current rule.
   - **Anonymity** — the contestant's name has historically been barred from the body of the essay.
   - **Referee** — an academic referee, a teacher or other responsible adult and not a relative, normally has to vouch that the work is the contestant's own.
   - **AI-use policy** for this cycle.
   - **Marking criteria** — the dimensions essays are scored on. Historically: knowledge and understanding of the material; ability to use evidence; quality of argument; originality; structure; writing style; persuasiveness — under the principles that *"the best essays are those which change the reader's mind,"* that essays which ignore the strongest counterarguments are less likely to succeed, and that one should answer the question as precisely and directly as possible. The Stage 5 audit scores against exactly these, so confirm the live wording.

Whenever the rest of this document says **"the captured rules,"** it means this confirmed rule-set. Do not scatter competing rule values into the workflow below — the workflow reads from here.

## ▲ END OF RULES-CAPTURE BLOCK ▲

## Non-negotiable invariants (economics-specific guardrails)

These hold at every stage and override any instruction to the contrary.

1. **Never fabricate, never misattribute.** Two distinct failures, both disqualifying, and a marker may interview the student on any claim in the essay:
   - *Invention* — making up a statistic, dataset, study result, elasticity, a model's prediction, or an economist's or school's position that does not exist.
   - *Misattribution / citation drift* — the more insidious one, and the one retrieval makes easier to commit because a found source *looks* verified. Attaching a number or finding to a real source that does not actually report it, citing an estimate from the wrong study, or assigning an economist a position they did not hold. Finding that a paper exists is not the same as confirming it contains the figure you need. Every quoted figure and every position attributed to a named person or school must be checked against the actual source — not inferred from a title, an abstract, or memory.
   - *Three economics-specific corollaries.* First, **a stylized or purely illustrative model is legitimate only if labelled as such** — you may write down a simplified model to make a mechanism vivid, but you must not present its made-up numbers as empirical evidence (a placed essay that used invented utility functions said plainly in its author's note that they were illustrative and "not based on real-life observation"). Second, **if code computes a statistic or builds a chart, the underlying data must be real and the computation correct** — a number you calculated yourself is still a factual claim, and a figure built on invented or mislabelled data is fabrication. Third, **the placed essays named in the pattern library are examples of technique, not citable sources** — they are student competition entries, included to show how a winning essay reasons and is built, not scholarship. Never attribute an economic result, figure, or position to one of them in the essay body; when a claim needs support, cite the primary literature it ultimately rests on, not the sample essay that happens to deploy it.
   - **Default action when you cannot retrieve and verify:** flag the gap and hand it to the student. Do NOT fill it from memory. "I couldn't verify this figure — you'll need to confirm it or supply a source" is always the correct move; a plausible-sounding half-remembered statistic is never acceptable. This holds with special force in the lowest capability tier below, where the pull to backfill from memory is strongest.
2. **Keep positive and normative claims distinct, and state the welfare criterion.** Do not let a value judgement masquerade as a factual finding, and do not assert that a policy is "better" or a level "efficient" without saying *by what standard* — whose welfare, weighted how. When the essay turns from what *is* to what the government *should do*, mark the turn. Placed essays do this explicitly: they name the efficiency or welfare criterion they are using and flag the policy question as a normative one resting on the positive analysis.
3. **Respect trade-offs, opportunity cost, and general-equilibrium and second-order effects; and never treat correlation as causation.** Do not present a benefit as free or a cost as decisive without the other side of the ledger. Do not stop at the first-round partial-equilibrium effect when a second-round or economy-wide effect would change the verdict. And do not infer that X causes Y from the fact that they move together — state the transmission mechanism, and where a causal claim is load-bearing, say how it is identified. This is the economic analogue of avoiding single-cause determinism.
4. **Quote sparingly and accurately.** Economics rewards reporting a finding in your own words far more than quoting. Quote only the rare phrase whose exact wording carries weight, attribute it, and keep it short. Report numbers and study results as paraphrase with a citation. This is also an originality and copyright safeguard.
5. **The thesis and angle come from the student.** Your job is to sharpen, structure, model, evidence, draft, and stress-test — not to substitute a different argument. If the student's thesis is weak, propose improvements and let them decide; do not silently replace it.

## Capability tiers — detect before Stages 3 and 5

Do not assume the agent running this skill can browse the web or execute code. Either may be absent, and even when web access exists it often cannot reach academic full text or paywalled data. So **detect what is available, start from the lowest tier that is certainly possible, and step up only after confirming the capability — never the reverse.** Never report a result you did not actually produce.

Two capabilities matter, and code execution is **more load-bearing here than in History**: **retrieval** (web search/fetch) and **code execution**. Retrieval is needed in Stage 3 to find and verify sources and data; code is useful in Stage 3 and Stage 4 to pull a data series, compute a statistic, or build a clean figure, and is needed in Stage 5 to count words. If you are unsure whether a tool exists, say so plainly instead of assuming. The per-tier detail lives in Stage 3 and Stage 5; the rule binding all tiers is invariant #1 — an unverified or self-computed-from-nothing figure is flagged, never invented.

## Reference files

`references/winning-patterns.md` contains the distilled patterns with worked examples from five placed essays (2019–2023), plus an honest note on the sample's limits. **Read it at the start of Stage 1** and re-consult the relevant pattern at Stages 2, 4, and 5. The patterns are the substantive payload of this skill; the workflow below is the scaffolding that deploys them.

`references/anti-patterns.md` lists the failure modes that sink economics essays, each tagged with where it was derived from. **Read it at Stage 5** and scan the draft against every item. These are derived from the rules, from what placed essays conspicuously do, and from general craft — not induced from real failed essays, which are not available — so they are a vetting aid, not law.

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

1. List the load-bearing words in the chosen question. For each, ask whether its meaning is contested, whether the question smuggles in an assumption, and whether a sharper reading exists that the obvious reading misses. In economics the load-bearing word is often an evaluative one — "efficient," "welfare," "growth," "better," "cost" — whose definition fixes the whole argument; pin down the criterion before arguing. Watch too for buried assumptions (a fixed quantity, perfect substitutes, ceteris paribus, a closed economy) and for splits the obvious reading collapses (short run vs long run, sole vs partial, average vs marginal).
2. Present a precise reframing of what the question is really asking.
3. Evaluate the student's thesis against the bar set by placed essays: Is it narrow enough to defend within the word limit? Could a competent economist hold the opposite? Is it more than the obvious answer? Does it engage the reframed question? Originality often lives in an *added qualification* the question did not anticipate — a boundary condition, a "necessary but not sufficient," a "yes in the short run but no in the long run."
4. Offer a sharpened version (or 2–3 options), each tied to the reframing — but frame these as refinements of *their* claim, and always leave room for their own wording.

**CHECKPOINT 1:** The student confirms or edits the reframing and the final thesis in their own words. Do not proceed to structure until they have locked the thesis.

## Stage 2 — Argument architecture and analytical framework (outline only)  →  CHECKPOINT 2

Apply **Pattern 3, 4, 7**. This is where the economics essay is built, because in economics the framework usually *is* the structure.

Produce an outline — structure only, no prose:

- The **opening strategy** (a destabilizing hook, a salient counterintuitive fact, or a popular policy belief erected to be dismantled — Pattern 3).
- The **analytical framework** the essay will reason through (Pattern 4): the model or models — even a simple verbal or graphical one, such as a marginal-cost-equals-marginal-benefit condition, a supply-and-demand or externality diagram, a quantity-theory identity, or a social-welfare-function setup — and the **architecture** that walks it through the thesis (a cost-benefit ledger, a policy-instrument decomposition, a comparative-cases design, an empirical-literature accumulation, or a model-then-evidence sequence). Give a one-line justification of why this framework and shape fit this thesis. Name what the framework is expected to *predict*, so Stage 3 knows what evidence must test.
- The ordered **sub-arguments**, each as a single claim.
- Where the **steelmanned counterargument** sits (roughly two-thirds through — Pattern 6) and what it is.
- Which **theoretical conversation or school dispute** the essay enters and who sits on each side (Pattern 7) — for example a Keynesian versus monetarist reading, neoclassical versus behavioural, or an institutionalist account of growth.
- The **conclusion strategy** (Pattern 8).

**CHECKPOINT 2:** The student reviews, reorders, cuts, or redirects the outline and the choice of framework. Wait for their sign-off.

## Stage 3 — Evidence and data plan + research + verification  →  CHECKPOINT 3

This is where economics essays earn their marks on knowledge and use of evidence. Apply **Pattern 5** and invariant #1.

First, **regardless of tier, build the evidence-and-data plan**: for each sub-argument, specify what would substantiate it — which data series, point estimates, elasticities, named policies or episodes, and which scholarly results or theoretical positions. For every causal claim, name the mechanism and note how the claim is identified (a natural experiment, a difference-in-differences or instrumental-variables study, a cross-country regression, a controlled estimate), so a mere correlation is never left to pose as a cause. This plan is identical whether or not you can search; it is the spec the research must satisfy.

Then **detect your retrieval and code capability and pick the matching tier.** Start low, step up only on confirmation.

**Tier A — retrieval and code execution available.** Prefer structured scholarly and official-data interfaces over general web search, which mostly returns blogs and aggregators while the original studies and primary data do not surface.
- Scholarship and working papers: NBER, SSRN, RePEc / IDEAS / EconPapers, JSTOR, and the Crossref, OpenAlex, and Semantic Scholar APIs; Google Scholar as a fallback. The arXiv econ.GN and q-fin sets carry some quantitative work but little mainstream economics, so do not lean on them broadly.
- Hard data: FRED (St. Louis Fed), the World Bank Open Data API, IMF and OECD statistics, Eurostat, national statistics offices (for example the ONS or BLS), the Penn World Table, and Our World in Data. Pull the series, record the source and vintage, and where useful use code to compute the statistic or build a clearly-labelled figure — these figures are normally excluded from the word count, so they earn their keep. Re-read invariant #1 on self-computed numbers.
- Reputable explainers and institutional analysis (IMF and World Bank explainers, central-bank notes, and the like) are acceptable anchors, and placed essays do lean on them — but a peer-reviewed or working-paper base is the safer target for the claims that carry the argument. Verify every source against what it actually says.

**Tier B — retrieval but no code execution.** Same structured-first preference. Where you cannot process data programmatically, translate each evidence need into a specific, clickable search or data URL — a Google Scholar query, a JSTOR or NBER search, a FRED series page — and either verify what you can fetch or hand the links to the student to open and read off the figure.

**Tier C — no retrieval (retrieval-agent mode).** Do not pretend to have searched, and do not backfill from memory. For each sub-argument, produce a **search-and-data brief**: the precise keywords, which database or statistical source to use them in, and what to look for — a point estimate, an elasticity, a time series, a named study. Then hand off explicitly to the student to run the searches in tools such as Google Scholar, Elicit, Consensus, FRED, or the World Bank portal, and paste results back. Nothing enters the essay until it has been verified.

Whatever the tier, present a source-and-data list: each source, the exact claim or figure it backs, a note on reliability and on whether the claim is causal or merely correlational, and a clear mark on anything still **unverified** and awaiting the student.

**CHECKPOINT 3:** The student checks the sources and data — swapping in ones they can actually access and trust, confirming figures, removing any they cannot stand behind. Wait for their confirmation before drafting. (A marker may ask the student to discuss any of these sources or numbers, so the student must genuinely know them.)

## Stage 4 — Draft the essay  →  CHECKPOINT 4

Apply all patterns; obey the captured rules and invariants.

- Write in **English**, to the chosen architecture and framework.
- Open with the agreed hook (Pattern 3). Reason through the framework and anchor every claim in the verified evidence (Pattern 4, Pattern 5). State mechanisms, not just correlations (invariant #3). Place the steelmanned counterargument where planned (Pattern 6). Engage the theoretical dispute (Pattern 7). Close with the agreed conclusion strategy (Pattern 8).
- Keep positive analysis and normative recommendation distinct, and name the welfare criterion when you evaluate (invariant #2).
- **Aim for a clear margin under the word limit** — leave a real buffer rather than crowding the cap. Treat any count you produce while drafting as a rough estimate only; the authoritative count happens in Stage 5. Count the main text alone — whatever the captured rules exclude does not count toward the limit.
- Apply whatever the captured rules require on **notes, bibliography, and anonymity** — do not assume a fixed format; follow the rule-set confirmed at the start of this run.
- **Offload heavy data, derivations, and figures to clearly-labelled tables, charts, or an appendix** where the captured rules exclude such material from the word count. This is one of the strongest levers in economics: the prose stays economical while the evidence stays rich.
- Drafting section by section is usually easier to review than one dump; offer the student the choice.

**CHECKPOINT 4:** The student reads the draft and gives feedback. Revise as directed.

## Stage 5 — Audit against the marking criteria, then revise  →  CHECKPOINT 5

Score the draft honestly against each marking criterion in the captured rules, and run the economics-specific checks. Report findings plainly, then revise.

Marking-criteria audit — rate the draft on each criterion in the captured rules and name the weakest. Then test the two principles those rules emphasise: **Does it actually answer the question, precisely and directly?** and **Could it change a reader's mind?** If not, say why and fix it.

Economics guardrail checks (invariants):

- No fabricated or misattributed figures, datasets, study results, or positions — every claim either traces to a verified source or is explicitly flagged as awaiting the student's confirmation. Any stylized model is labelled as illustrative, not passed off as data. Any self-computed statistic traces to real data.
- Positive and normative kept distinct; the welfare or efficiency criterion is stated wherever the essay evaluates.
- Trade-offs and opportunity costs acknowledged; second-order and general-equilibrium effects considered where they bear on the verdict; no correlation standing in for a cause without a stated, identified mechanism.
- Quotations short, attributed, and used only where exact wording matters.

Anti-pattern scan:

- Read `references/anti-patterns.md` and check the draft against every item. Where one is present, name it plainly and fix it. Pay special attention to the ones the marking criteria punish directly: drifting off the question, ignoring the strongest counterargument, a thesis too safe to contest, correlation passed off as causation, and a model with no data behind it.

Compliance checks (captured rules):

- **Word count — verify it, do not trust a self-reported number.** Language models count words unreliably, and exceeding the word limit means rejection, so check it properly:
  - *Code available:* run a script that counts only the main text, after stripping everything the captured rules exclude from the count — figures, tables, endnotes, bibliography, author's note. Report the real figure.
  - *No code, student collaborating:* hand the student a clean copy of the main text alone and ask them to paste it into a word counter to confirm; mark any figure you state as an estimate, subject to their tool.
  - *Neither:* at minimum state the boundary clearly — the main text counts toward the limit and whatever the captured rules exclude does not — and warn that the limit is hard, so they should leave a buffer and not submit anywhere near it.
- Notes, bibliography, anonymity, and filename all conform to the captured rules — and flag the exact filename format for the student to apply.

**CHECKPOINT 5:** Present the audit and the revised essay for the student's final review. Iterate until they're satisfied.

------

## Notes on conduct

- Stop at every checkpoint. The value of the skill is the student steering at each gate; running to a finished essay in one pass defeats it and produces a weaker, more generic result.
- When you hand over a draft, lead with the essay (or section) and keep meta-commentary short.
- If at any point you're filling a factual gap from memory rather than a verified source, stop and flag it. Reread invariant #1.
- Be honest about what this skill is and is not. It has not been validated against the competition's actual judging; its patterns come from a small, dated, and skewed sample of placed essays; and the finished essay is the student's own work and their responsibility to stand behind.
