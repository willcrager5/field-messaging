# Field Messaging Plugin

A Claude Code plugin for Field's brand, messaging, and positioning work. Available to the full Field team.

## What's in here

**Field Brand Strategist agent** — A named brand strategist for any Field team member. Introduces itself on first use, reads content from a shared bucket, weights recent content heavier than older content, and drives messaging framework work with Field-specific context already loaded. Bill is the final decider on all working positions.

**Brand Voice skill** — Generate new content in Field's voice or review existing content against brand voice, vocabulary rules, and working positions. Works for any surface: LinkedIn posts, emails, deck copy, website sections, one-pagers, press boilerplate, Slack announcements, event bios.

**Messaging Framework skill** — The 10-section framework (Category, Ecosystem Narrative, Brand Architecture, Messaging Pillars, Segment Messaging, Persona Value Props, Competitive Positioning, Tone/Language/Vocabulary, Elevator Pitches, Objection Handling). Primary mode is content extraction — mine existing content, draft the framework, react and refine.

**Banned Phrases master list** — Single source of truth for all vocabulary enforcement. 80+ hard-banned words with replacements, 11 banned expression patterns with approved rewrites, and style rules. Loaded automatically by every skill and the agent.

**Field ecosystem decisions** — Reference file with all working positions: category (Modern Wealth Intelligence), tagline (Common ground. Build on it.), architecture (Translation → Comprehension → Fluency), five pillars, four outcomes, BridgeFT S3 locked. May 6, 2026. Bill is the decider on all open items.

**Anti-AI tells guide** — Enforcement reference for review sessions. Structural, reasoning, sentence-level, and opener/closer patterns that reveal AI authorship even when vocabulary is clean. Loaded in Review mode before banned-phrases.

**Voice Enforcement skill** — Load at session start to make the anti-AI tells, the banned-phrases list, and a before/after pattern library active constraints for the rest of the session. Three parts: Part A (Field's anti-AI tells), Part B (banned phrases and hard-ban expression patterns), and Part C (a 33-pattern library with before/after examples adapted from Wikipedia's "Signs of AI writing," tuned to Field's surfaces and cross-referenced against A and B so nothing is enforced twice). Adds a draft → audit → final rewrite loop. Trigger phrases include "load enforcement," "apply Field voice rules," and "humanize this."

**RIA segment messaging** — Approved language for both $15B+ and $1-15B registers. Lead narratives, positioning statements, layer-to-theme mapping, and what-not-to-say guidance. Loaded for any RIA-facing content.

---

## How to install

### Prerequisites
- Claude Code installed and running
- Access to a Cowork workspace (or a local folder you point Claude Code at)

### Install command

In Claude Code, run:

```
/plugin install willcrager5/field-messaging
```

That's it. No re-install needed for future updates — pull the latest from GitHub and the plugin updates automatically on the next session.

### Verify it worked

After installing, you should see:
- `messaging-strategist` available as an agent
- `brand-voice` and `messaging-framework` available as skills

---

## How to use it

### For content generation or review (most common)
Use the **brand-voice** skill. Tell it what you're writing, who it's for, and what you want. It will load the current working positions and banned phrases automatically and either draft or review the content.

### For messaging framework work
Use the **messaging-strategist** agent. Drop content into `Brand/Bill-Content/` at your Cowork workspace root — LinkedIn posts, deck slides, memos, transcripts, anything. The agent reads it, extracts patterns, and works through the framework with you. Date filenames `YYYY-MM-DD-short-description.md`. No other organization required.

### For checking what's banned
Open `skills/messaging-framework/references/banned-phrases.md` directly. Every banned word, every banned expression pattern, and every approved replacement is there.

---

## How the agent works

- Reads the full content bucket on first ask, recency-weighted
- Updates `Brand/Bill-Content/_log.md` after each session so the messaging journey is visible over time
- Cites source files when it extracts a pattern
- Pushes back on banned phrases, cheap language, and data-forward advisor copy
- Produces artifacts to `Brand/Drafts/`, `Brand/Messaging-Framework/`, and `Brand/Decisions/`
- Asks one question at the end of each session to capture any position shifts

---

## What the agent doesn't do

- Edit the messaging-framework skill itself (maintained separately)
- Visual design work
- Non-messaging tasks

---

## Updating the plugin

Pull the latest from GitHub:

```bash
git pull
```

No re-install needed. The plugin picks up changes automatically on the next session.

---

## Maintaining it

To add or remove a banned word or phrase: edit `skills/messaging-framework/references/banned-phrases.md` only. All skills and the agent load from that one file — nothing else needs to change.

To update working positions: edit `skills/messaging-framework/references/field-ecosystem-decisions.md`. Log the change in `Brand/Bill-Content/_decisions-log.md` with before/after and Bill's reasoning.

Maintained by Will (cragerw). Commit and push — the repo is the source of truth.
