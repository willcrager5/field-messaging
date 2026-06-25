# Scheduling the brief

One scheduled task drives this skill. Set it up once using the `schedule` skill.

## Weekly Monday lookahead

- **When:** Mondays at 8:00 AM local time
- **Task prompt:** "Run the `bill-launch-brief` skill. Read `Brand/Field-Brand-Launch-Critical-Path-Updated.xlsx`, filter Bill-owned tasks, and write the brief to `Brand/Bills-Briefs/`. If a Slack connector is configured, DM the brief to Bill. Otherwise, present the file."
- **Stop condition:** After May 5, 2026 (the launch date). Retire the schedule post-launch.

## Delivery paths

Default: file output in `Brand/Bills-Briefs/YYYY-MM-DD-weekly.md`. The brief is already Slack-compatible Markdown (headers, bold, bullets), so once a Slack MCP connector is wired into the workspace, extend the scheduled task to also post the brief as a DM to Bill.

If no Slack connector is configured, note this once and move on — don't re-prompt every run.
