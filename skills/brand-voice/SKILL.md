---
name: brand-voice
description: |
  Generate new Field-branded content or review existing content against Field's brand voice and working messaging positions. Use this skill when the user wants to draft, write, or produce any asset — LinkedIn posts, email sequences, sales deck copy, website sections, one-pagers, pitch language, event bios, press boilerplates, Slack announcements, conference booth copy, outreach emails. Also use when reviewing, auditing, or QA-ing existing content for voice, tone, vocabulary, and positioning accuracy. Trigger phrases: "write this," "draft," "does this sound right," "is this on-brand," "review this," "check this copy," "help me say this," "how would Field say this," "can you write a LinkedIn post." This skill applies the messaging framework — it doesn't rebuild it. If a positioning question surfaces here, flag it and route to messaging-framework or escalate to Bill.
---

# Brand Voice — Generate & Review

## What This Skill Does

Two jobs:

1. **Generate** — Draft content in Field's brand voice for any surface or format, grounded in the current working messaging positions.
2. **Review** — Audit existing content against the brand voice, vocabulary rules, and working positions. Return flagged issues and a clean revised version.

This skill applies what's already been decided. It doesn't re-litigate positioning. If the user surfaces a positioning question while using this skill, flag it and route it to the messaging-framework skill or flag it for Bill.

---

## What to Load Before Running

Before generating or reviewing anything, load all three:

1. **Working positions** — `skills/messaging-framework/references/field-ecosystem-decisions.md`. Active decisions on category, product suite, pillars, vocabulary, sequencing, and brand architecture. Do not skip this.
2. **Agent context** — The "Working Positions" section of `agents/field-brand-strategist.md`. Shorthand flags and active rules; faster to apply than the full reference document.
3. **Banned phrases — master list** — `skills/messaging-framework/references/banned-phrases.md`. The single source of truth for every banned word, banned expression pattern, and style rule. Load it. Enforce every item in every output. Nothing slips through.

If any source has been updated since the last session, the new version takes precedence.

---

## Mode 1: Generate

### Before drafting, establish

- **Surface** — What is this for? (LinkedIn post, email subject line, email body, deck slide headline, hero copy, one-pager section, event bio, press boilerplate, pitch intro, sales email, Slack announcement, etc.)
- **Audience** — Who reads it? (RIA firm principal, lead advisor, COO/ops leader, asset manager, developer, investor, internal team, press)
- **Goal** — What should they do or believe after reading? (book a demo, understand the product, feel confident in a partnership, approve a decision, share it)
- **Context** — What's happening around it? (product launch, outreach campaign, event, internal milestone, announcement, post-meeting follow-up)

If the user hasn't provided these, ask once — briefly. Don't interrogate. Make reasonable inferences when context is clear and state what you assumed.

---

### Voice rules

**The voice in three words: Plainspoken. Confident. Human.**

Field's brand voice is Bill's voice — sharp, experienced advisor-turned-operator, not a software vendor. These rules hold across all surfaces:

**Always:**
- Plain-spoken and direct. Short sentences. No throat-clearing.
- Peer register. Speak like someone who has been in the room.
- Lead with outcomes, not features or capabilities.
- Concrete and specific — name the thing. Be specific, not sweeping. "Fifteen thousand firms. Five hundred fifty platforms." Real numbers land harder than abstractions.
- Acknowledge the human cost. This isn't a technology problem. It's a people problem. The advisor is the person paying the price. Never let the infrastructure language crowd out the human stakes.
- Arrive at the point. Field doesn't wind up. It states. The period earns its place.
- Sequencing matters: lead RIA, reveal Network. Never pitch all three audiences on one surface.
- Make claims. Don't hedge into passivity.

**Never use:**
The complete banned-word and banned-pattern list is in `skills/messaging-framework/references/banned-phrases.md`. It must be loaded before any generate or review session (see "What to Load Before Running" above). Enforce every item. Do not rely on memory or a partial inline list.

Specific Field-brand additions not in the master list:
- "Ecosystem" in formal brand language — use "platform" or "network" per the vocabulary rule
- Questions as headlines — make a claim instead
- Timid hedges: "We hope to help firms potentially improve their workflows"
- Generic SaaS openers ("Are you struggling with...?" / "In today's fast-paced world...")

**Use deliberately (context rules apply):**
- "Advisor-owned" — only after governance model has been stated or is visible in context. Not in cold outreach or first-touch.
- "Field Network" — strategic context only. Not on RIA-facing surfaces where the network hasn't been introduced.
- Product name for the data layer — use the locked name once it's decided; use "data foundation" or "intelligence layer" until then.
- "Foundation" naming candidates — hold off on any candidate name until Bill has decided.

**Brand vocabulary quick reference:**
- "Field Platform" = the software. Use on RIA-facing surfaces.
- "Field Network" = the multi-sided system. Strategic context, investor decks, ecosystem narrative — not RIA homepage.
- "Modern Wealth Infrastructure" = the category name. Replaces "Field Wealth Intelligence" and "Wealth Intelligence Network."
- BridgeFT: currently in Phase 1 light endorsement. Endorsed form: "BridgeFT, part of Field." Not yet "Field WealthTech API" on external surfaces.
- Precept: same phasing pattern as BridgeFT. Details TBD with Bill — hold until clarified.
- "Luca" = internal pipeline name only. Never customer-facing.

---

### Output format

Produce the draft. Below it, add a brief **Voice notes** block (3–5 lines max):
- The key choice made (angle, lead, register, what was cut)
- Any vocabulary calls that weren't obvious
- One thing to change if it doesn't feel right

Don't explain every sentence. Flag only the choices worth reviewing.

---

### Surface-specific rules

**LinkedIn (Bill's voice):**
- Personal, first-person. This is Bill talking, not Field the company.
- Plain opener — no "Excited to announce." Open with the thing itself.
- Short paragraphs, one idea each. Line breaks are structure, not decoration.
- End with a question or a specific observation — not a demo CTA.
- No emoji unless user asks. No hashtags in the body.
- 150–250 words is the right range for most posts.

**Sales email / outreach:**
- Subject line: specific, earned. Name the problem or outcome — not a teaser.
- Body: four sentences max before the ask. State who you are, what they get, why now, what you're asking.
- No "I hope this finds you well."
- The ask is one specific action.
- Personalize the first line to something real about the recipient's firm, not a generic opener.

**Deck slide copy:**
- Headlines are claims, not category labels. "Field unifies the data stack" not "Platform Overview."
- One idea per slide.
- Bullets: max four, each under 12 words.
- No full sentences in bullets unless it's a direct quote or a key phrase meant to stand alone.
- Slide titles and bullets should be able to read independently from any body text.

**Website / hero copy:**
- The hero is for RIAs. Everything else is navigation.
- Lead with outcome, not product description.
- Six-word frame is a valid test — "See your firm. Finally." is a live candidate.
- CTA is specific: "Book a demo," "See how it works" — not "Learn more."
- No category jargon in the first two lines. Earn the terminology.

**Press / boilerplate:**
- Short boilerplate: one sentence. What Field does, for whom.
- Long boilerplate: 3–4 sentences. Category claim → product → proof point → ecosystem context.
- First-mention rule: if BridgeFT appears, pair with endorser line on first mention ("BridgeFT, part of Field"), then sub-brand alone thereafter.
- No hype language. State the claim plainly. Press will quote it verbatim — make it defensible.

**Event bio (Bill):**
- Third person, 3–5 sentences.
- Open with what Bill built or the problem he's spent his career on — not his title.
- Include Field + BridgeFT acquisition context in one line.
- End with one sentence that sounds like a real person said it, not a LinkedIn summary.

**Internal / Slack announcements:**
- Still Field voice — no corporate-speak.
- State the thing directly: what happened, what it means, what's next.
- Avoid passive constructions. "We signed X" not "X has been signed."

---

## Mode 2: Review

### What review checks

Run content through four lenses:

1. **Banned phrases** — Load `skills/messaging-framework/references/banned-phrases.md` and check every word and expression pattern against the master list. This is the first pass, not an afterthought. Flag every hit by name.
2. **Voice** — Does it sound like Field? Peer register? Any throat-clearing, vendor-speak, or generic SaaS phrases?
3. **Vocabulary** — Are the vocabulary rules being followed? Check: avoid/never words, architecture words (platform vs. network vs. ecosystem), product names at the correct phase, BridgeFT/Precept endorser lines.
4. **Positioning accuracy** — Does it reflect current working positions? Check: category claim, product suite (four offerings — correct names and scopes), audience sequencing (RIA-first), pillar alignment.
5. **Sequencing** — Right message for this surface and audience? Would the wrong audience be confused or misled?

### Output format

1. **Overall verdict** — Pass / Needs work / Significant issues. One line.
2. **Issues** — Bulleted. Each issue: *the specific text* → what's wrong → suggested fix. Grouped by lens.
3. **Clean version** — Revised draft applying all fixes. If mostly good, revise with changes inline. If significantly off, produce a fresh draft.

Keep the issues list tight. Flag things that materially contradict voice rules, vocabulary rules, or working positions. Don't flag minor style preferences as violations.

---

## What This Skill Does Not Do

- **Does not revisit positioning.** If a review surfaces a positioning question ("is this claim still accurate?"), flag it for messaging-framework or Bill. Don't resolve it here.
- **Does not override Bill.** If Bill has explicitly approved language that this skill would flag, defer. Note the tension, don't override.
- **Does not generate legal, compliance, or regulatory language.** Route to Andy/legal.
- **Does not write content for competitive entities** — Field voice only.