# Field messaging — decisions log

Append-only record of every shift in Field's messaging positions. Each entry captures what changed, why, and where the change landed. Older entries are never edited or deleted — they're the historical record of how Bill's thinking moved.

The agent writes to this file at the end of any session where a position shifted. Will can add entries manually when a shift happens outside a session.

---

## YYYY-MM-DD — [short title of the shift]

**Before:** [exact prior phrasing, quoted from the reference file]

**After:** [exact new phrasing]

**Bill's reasoning:** "[direct quote, paraphrased only if necessary]"

**Files touched:** [list of reference files edited]

---

## Example (delete when real entries begin)

## 2026-04-14 — Dropped "Wealth Intelligence Network" as strategic register

**Before:** Category (strategic register) — working: "We're building the Wealth Intelligence Network"

**After:** Category (strategic register) — working: "We're building the Wealth Intelligence Layer"

**Bill's reasoning:** "Network sounds like LinkedIn. Layer is more honest — we sit on top of everyone else's infrastructure, we don't replace it."

**Files touched:** `skills/messaging-framework/references/field-ecosystem-decisions.md`
