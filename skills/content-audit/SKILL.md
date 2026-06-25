---
name: content-audit
description: |
  Run a comprehensive diagnostic on any piece of Field content before it goes out. Use when you want to know what's wrong before sending to Bill, before publishing, before a deck goes to a prospect, or any time content feels off but you can't pinpoint why. Accepts any format: LinkedIn posts, email copy, deck slides, website sections, one-pagers, press boilerplates, sales emails, event bios, outreach sequences. Returns a structured audit report: AI-tell violations, banned phrase hits, working-position conflicts, and an overall verdict. Trigger phrases: "audit this," "check this before I send it," "what's wrong with this," "is this ready," "QA this," "review before approval," "does this pass."
---

# Content Audit

## What This Skill Does

One-pass diagnostic on a single piece of content. Three sequential checks, one structured output. The goal is a clear verdict with specific callouts — not a rewrite (that's `brand-voice`), not a session-wide enforcement mode (that's `voice-enforcement`), just a fast, complete diagnostic.

Use this before content leaves the building.

---

## What to Load Before Running

Load these three files before auditing anything:

1. **Anti-AI tells** — `skills/messaging-framework/references/anti-ai-tells.md`. Run this check first. AI writing can pass every vocabulary rule and still read like AI. The tells are structural, rhythmic, and reasoning-level — not just word choice.
2. **Banned phrases** — `skills/messaging-framework/references/banned-phrases.md`. The single source of truth for banned words, banned expression patterns, and style rules. Every item applies.
3. **Working positions** — The "Working Positions" section of `agents/messaging-strategist.md`. Active decisions on category, tagline, architecture, pillars, vocabulary, and sequencing.

Do not audit without loading all three.

---

## What to Establish Before Starting

Ask the user once — briefly — if they haven't already said:

- **Surface** — What is this? (LinkedIn post, email, deck slide, one-pager, homepage section, bio, press quote, etc.)
- **Audience** — Who reads it? (RIA firm principal, advisor, asset manager, investor, internal team, press)

If context is obvious from the content itself, make the inference and state it. Don't interrogate.

---

## The Three Checks

Run in this order. Don't skip ahead.

### Check 1: AI Tells

Load `anti-ai-tells.md`. Go through every pattern in that file — structural, reasoning-level, sentence-level, opener/closer — and flag every hit.

For each violation:
- Quote the offending text exactly
- Name the pattern (e.g., "epoch-framing opener," "stacked-noun-phrase," "aspirational closer")
- State the problem in one sentence
- Propose a specific fix or rewrite direction

This check catches what vocabulary enforcement misses. A clean vocabulary pass doesn't mean the writing is human. Run this first, before banned phrases, every time.

### Check 2: Banned Phrases

Load `banned-phrases.md`. Check every word, every expression pattern, every style rule. No exceptions, no "close enough."

For each violation:
- Quote the offending text exactly
- Name the ban category (hard-ban word, hard-ban expression pattern, style rule)
- Give the approved replacement

If the same word appears multiple times, list each instance — don't summarize.

### Check 3: Framework Alignment

Load the working positions from `agents/messaging-strategist.md`. Check the content against:

- **Category** — Does it use the right category name (Modern Wealth Intelligence)? Does it create a different category or blur it?
- **Tagline / supporting line** — Used correctly? Misquoted? Used in a context where it doesn't land?
- **Architecture** — Translation → Comprehension → Fluency. If referenced, is it accurate?
- **Vocabulary rules** — Field Platform vs. Field Network. Correct register? No "ecosystem" in formal brand language?
- **Audience sequencing** — Does this RIA-facing content accidentally pitch multiple audiences? Does it lead with the network story instead of the platform?
- **BridgeFT / Bridge naming** — Correct endorsed form ("Bridge, a Field product")? "BridgeFT" used where it shouldn't be?
- **Pillar alignment** — If pillars are invoked, are they the correct five? In the right language?
- **Claims** — Any claim that's unsupported by the working positions or that contradicts a locked decision?

For each issue:
- Quote the offending text
- Name the working position it violates or conflicts with
- State the correct version

---

## The Audit Report

Always produce the report in this structure. Never summarize into prose — the structured format is the deliverable.

```
## Content Audit — [Surface] for [Audience]
[One line: what you audited]

### Verdict
PASS | LIGHT EDITS | HEAVY REVISION

[One sentence on the overall state. Honest.]

---

### Check 1: AI Tells
[CLEAN or list of findings]

**Finding 1**
> "[exact quote]"
Pattern: [name from anti-ai-tells.md]
Problem: [one sentence]
Fix: [specific rewrite direction or example]

...

---

### Check 2: Banned Phrases
[CLEAN or list of findings]

**Finding 1**
> "[exact quote]"
Ban type: [hard-ban word / expression pattern / style rule]
Replace with: [approved replacement]

...

---

### Check 3: Framework Alignment
[CLEAN or list of findings]

**Finding 1**
> "[exact quote]"
Issue: [what position it violates or conflicts with]
Correct: [what it should say]

...

---

### Summary
[2-3 sentences. What's the most important thing to fix, and why. Be direct.]
```

**Verdict definitions:**
- **PASS** — No findings, or only 1–2 minor style flags that don't affect meaning
- **LIGHT EDITS** — Fixable issues; the structure and positioning are sound; clean up takes minutes
- **HEAVY REVISION** — Multiple framework conflicts, significant AI-tell patterns, or systemic banned-phrase violations; the piece needs a full pass before it goes out

---

## After the Report

Do not offer to rewrite automatically. Ask once:

> "Want a clean version with all of these fixed, or do you want to take the findings and revise it yourself?"

If they want the clean version, rewrite it applying all findings. Apply the voice-enforcement rules as live constraints — this is generate mode, not review mode. Don't produce a clean version that introduces new violations.

If they want to revise it themselves, stop. Don't coach them through every line unless they ask.

---

## What This Skill Does Not Do

- It does not rebuild the messaging framework. If auditing reveals a strategic positioning problem, flag it and route to `messaging-framework` or escalate to Bill.
- It does not make judgment calls on open working positions. If a position is marked open, note it as a watch item, not a violation.
- It does not audit an entire content library. For batch audits, run separately on each piece.
