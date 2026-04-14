# Field Brand

A private plugin for Field's brand, messaging, and positioning work. Built for Bill.

## What's in here

**Field Brand Strategist agent** — A named brand strategist Bill talks to. Introduces itself on first use, reads Bill's content from a single bucket, weights recent content heavier than older content, and drives messaging framework work with Field-specific context already loaded.

**Messaging Framework skill** — The 10-section framework (Category, Ecosystem Narrative, Brand Architecture, Messaging Pillars, Segment Messaging, Persona Value Props, Competitive Positioning, Tone/Language/Vocabulary, Elevator Pitches, Objection Handling). Primary mode is content extraction — mine existing content, draft the framework, let Bill react.

**Field ecosystem decisions** — Reference file with the working positions: category register map, RIA narrative lead, governance/subsidy model, Platform vs. Network vocabulary rule, BridgeFT phased transition. Nothing is locked — Bill is the decider.

**Wealth ecosystem map** — Terrain reference. Thirteen layers of the wealth stack, key players in each, Field's relationship to each. Loaded when positioning, competitive, or segment work comes up.

**Bill's Launch Brief skill** — Reads `Brand/Field-Brand-Launch-Critical-Path-Updated.xlsx`, filters Bill-owned tasks across all detail sheets, and generates a Field Brand Strategist-voiced weekly Monday brief. Output lands in `Brand/Bills-Briefs/YYYY-MM-DD-weekly.md`. Schedule it once with the `schedule` skill (see `skills/bill-launch-brief/references/schedule-setup.md`); Slack DM delivery can be added when a Slack connector is wired.

## How Bill uses it

1. Drop content into `Brand/Bill-Content/` at the Cowork workspace root. Date filenames `YYYY-MM-DD-short-description.md`. Everything goes in one folder — no organization required.
2. Open a session. The agent introduces itself.
3. Tell the agent what you want to work on, or let it read your content and tell you what it sees.

## What the agent does

- Reads the full content bucket on first ask, recency-weighted
- Updates `Brand/Bill-Content/_log.md` after each session so the messaging journey is visible over time
- Cites source files when it extracts a pattern
- Pushes back on cheap phrases and data-forward language
- Produces artifacts to `Brand/Drafts/`, `Brand/Messaging-Framework/`, and `Brand/Decisions/`
- Uses Bill's workspace naming conventions throughout

## What the agent doesn't do

- Edit the messaging framework skill itself (maintained separately)
- Visual design work
- Non-messaging tasks

## Installing

In Cowork, install from this repo:

```
/plugin install cragerw/field-brand
```

Or drag-and-drop the packaged `.plugin` file into Cowork's plugin panel.

Requires a Cowork workspace pointing at a folder with `Brand/Bill-Content/` (or the agent will create it on first run). Shared setups should sync the workspace via OneDrive, Dropbox, or Google Drive.

## Updating

Pull from this repo — Cowork picks up the new version automatically on next session. No re-install required.

## Maintained by

Will (cragerw). Update the agent's voice, the skill's sections, or the ecosystem decisions reference directly, commit, push. The repo is the source of truth.
