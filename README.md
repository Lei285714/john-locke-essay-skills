# John Locke Essay Skills

English | [简体中文](README.zh-CN.md)

A set of Skills designed for writing essays for the John Locke Institute competition.
 Through a staged, fully human‑in‑the‑loop workflow, it applies judgment methods distilled from past placed essays to your own writing process.

**Actively updated.** The History and Economics categories are now available. More categories will be added, and the existing ones will continue to be refined.

> Before relying on anything produced by this skill, please read the **Disclaimers** section.
> Note that this skill has **never** been evaluated by real John Locke judges, and the essays it draws from come only from a few past years.

## What it does

This repository provides collaborative writing workflows for specific categories (such as `john-locke-history-essay` and `john-locke-economic-essay`).
 You provide the question and a rough thesis; the skill moves them through five checkpointed stages — sharpening the thesis, designing the argument structure, planning and verifying evidence, drafting, and finally auditing against the marking criteria — applying techniques reverse‑engineered from past placed essays.
 It pauses at every checkpoint, so you remain in control throughout.

## Skills included in this repository

- **`john-locke-history-essay`** — History category, available now.
- **`john-locke-economic-essay`** — Economics category, available now.

Planned categories are listed under **Roadmap**.

## Repository structure

```text
.
├── LICENSE
├── README.md
├── README.zh-CN.md
├── john-locke-economic-essay/
│   ├── SKILL.md                  # Workflow: stages, checkpoints, guardrails
│   └── references/
│       ├── winning-patterns.md   # Judgment patterns distilled from Economics essays
│       └── anti-patterns.md      # Failure modes for scanning an Economics draft
└── john-locke-history-essay/
    ├── SKILL.md                  # Workflow: stages, checkpoints, guardrails
    └── references/
        ├── winning-patterns.md   # 8 judgment patterns distilled from History essays
        └── anti-patterns.md      # 12 failure modes for scanning a History draft
```

`SKILL.md` in each category is the skeleton; the reference files are the substance.

The skill loads `winning-patterns.md` at the start, and during the audit stage it checks the draft against `anti-patterns.md`.

## What you need to provide

This skill does **not** hard‑code any year’s competition rules, because they change every cycle.

At the start of each run, it checks whether you have supplied the current rules; if not, it stops and asks for them.

Prepare the following, copied verbatim from the official John Locke Institute page for the current cycle:

- the full list of questions for your chosen category (History or Economics), exactly as published
- the word limit, and what is excluded from the count
- submission requirements: filename format, citation and notes rules, anonymity, academic referee requirement, and the **AI‑use policy** for the year（Please do not **delete or modify some rules**）
- the marking criteria

You must also provide two things of your own:

- the specific question you have chosen
- your own rough thesis

The skill helps refine your idea, build the structure, assemble evidence, and stress‑test the argument.

It will **not** invent a thesis for you, nor choose the question on your behalf.

## How to use it

Use it in any product that supports Agent Skills.

Start a conversation about your John Locke essay (History or Economics category), paste in the current year’s rules when prompted, and proceed through the checkpoints one by one.

You may speak in any language; the essay itself will always be written in English.

## Disclaimers

Please read this section before trusting anything produced by the skill.

**Not validated by real judges.** Essays produced with this skill have never been evaluated by the John Locke Institute or by any human marker.

The only evaluation so far has been internal: several large language models blind‑compared drafts produced with the skill against past placed essays, and the models tended to rate the skill‑assisted drafts higher.

**This does not indicate anything real.** Model preferences do not predict human judgment. Treat the skill as a drafting and self‑critique tool, not a path to winning.

**Small and dated sample.** The techniques are reverse‑engineered from a small number of placed essays from the 2019, 2020, 2021, 2023, and other past cycles.

Question styles, judging priorities, and even the rules themselves may have changed.

What won then may not win now.

These patterns are only a starting prior, never a formula.

**You are responsible for the final essay.** The skill flags unverified claims, but you must confirm every source, fact, and quotation yourself, stay within the word limit, and follow the submission rules.

**This skill has not been tested across all models.** Different models may behave differently; always double‑check the output.

**For practice and research only. Do not submit essays produced by this skill directly to the official competition.**

## Attribution and copyright

The analysis, workflow, and technique write‑ups in this repository are independent educational commentary.

This project is **not affiliated with, authorized by, or endorsed by** the John Locke Institute or by any of the referenced essay authors.

The reference files mention and briefly discuss past placed essays solely for criticism and study, quoting only very short fragments when necessary for analysis.

Competition questions and marking‑criteria text belong to the John Locke Institute.

If you are an author referenced in the materials and would like your name or any quotation removed, please open an issue and it will be removed.

## Roadmap

- Expand into more categories beyond History and Economics, such as Law, Philosophy, etc.
- Continue refining the technique library for each category as more placed essays become available
- Improve evaluation methods to avoid relying on LLMs grading LLM‑assisted drafts

This repository is actively updated; structure and content may change.