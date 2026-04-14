---
name: bill-launch-brief
description: Generate a weekly Monday brief for Bill listing his outstanding brand-launch tasks. Use on cadence ("weekly brief for Bill", "Monday brief") or on demand ("what's on Bill's plate this week"). Reads the brand launch spreadsheet, filters Bill-owned tasks, and writes a Field Brand Strategist-voiced brief to the Bills-Briefs folder.
---

# Bill's Launch Brief

Generates a short, plain-spoken weekly brief for Bill listing the tasks assigned to him in the Field Brand Launch critical-path spreadsheet. One mode only: **Monday lookahead** — what slipped, what's on his plate this week, what's coming next week, and the one thing to move today.

The brief is written in **Field Brand Strategist voice** — direct, plain-spoken, no hedging, no cheap phrases. Bill is the decider; this is a reminder, not a lecture.

## Source

Single source of truth: `Brand/Field-Brand-Launch-Critical-Path-Updated.xlsx` at the Cowork workspace root. Resolve paths relative to the workspace root at runtime — do not hardcode session paths.

The spreadsheet has 11 sheets. Detail sheets have headers at row 3: `#, Task, Due Date, Status, Owner, Depends On, Notes`. The "Critical Path" summary tab is skipped because its items duplicate the detail tabs. Filter where `Owner` contains "Bill" (case-insensitive — catches "Bill", "Bill / Will", "Bill / Craig / Andy", etc.). Skip tasks whose Status is Complete/Completed/Done.

## How to run

```bash
# Use the Cowork workspace root as the path base. The plugin's skill dir is the caller's path.
python3 "${CLAUDE_PLUGIN_ROOT}/skills/bill-launch-brief/scripts/generate_brief.py" \
  --xlsx "Brand/Field-Brand-Launch-Critical-Path-Updated.xlsx" \
  --out  "Brand/Bills-Briefs"
```

The agent should run this from the workspace root (Bill's selected Cowork folder) so relative paths resolve correctly.

After the script runs, review the draft and apply the voice rules in `references/voice-rules.md` — strip any hedging, make sure the opener doesn't repeat what Bill already knows, and confirm the push picks the single highest-leverage task.

## Delivery

Default: file output in `Brand/Bills-Briefs/YYYY-MM-DD-weekly.md`, presented via `present_files`. If a Slack MCP connector is configured, also DM the brief to Bill. If no Slack connector is wired, note it once in the session and default to the file.

## Cadence

One scheduled task: **Mondays at 8:00 AM local**. Retire after May 5, 2026 (launch). Setup in `references/schedule-setup.md`.

## Structure of the brief

1. **One-line frame.** "N days to launch." No preamble beyond that.
2. **Slipped.** Anything overdue, called out — don't bury it.
3. **This week.** Grouped by urgency, not by sheet.
4. **Next week — get ahead.** Preview of what's coming.
5. **The one to move today.** A single specific push. Biased toward messaging/positioning work because that's Bill's highest-leverage contribution and everything downstream waits on it.

One screen. If the open-task list is long, the brief picks the items that matter this week.

## Voice rules (short)

Full rules in `references/voice-rules.md`.

- Direct, plain-spoken, peer voice.
- Never "disruptive," "supercharge," "just a heads up," "circling back."
- Open with the frame, not "Good morning Bill."
- Task name is usually enough. Add a one-line reminder from the `Notes` column only if the task name is vague.
- End with a specific push.

## What this skill does not do

- Does not edit the spreadsheet.
- Does not chase status from other owners.
- Does not run unsolicited. Only runs on Monday or on demand.
