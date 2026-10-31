# SuperDot routines and maintenance schedule

Version: 1.0.0 · 2026-10-31 · Template: suggested times, not active tasks

Copy this file to the private vault's `System/SCHEDULE.md` during setup. Personalise it there;
future package updates must not reset the person's choices. Use
[Scheduling](skills/scheduling/SKILL.md) to create native routines only after the relevant choices
are accepted. No live schedule is created by this document.

## Choices to confirm

- Timezone: EDIT — use the person's named local timezone; do not assume the builder's timezone.
- Delivery: EDIT — chosen private destination/channel; keep personal reports out of public sharing.
- Chosen Mac and vault: EDIT — actual authorised host/path.
- Review scope: EDIT — relevant vault areas, Notion pages and project folders.
- Storage scope: EDIT — approved folders/volume; excludes secret stores and unapproved system areas.

## Suggested starting schedule

These are editable defaults for a person to accept, change or skip. All rows start **proposed**.
One confirmation may cover the chosen set, timezone, scope and delivery; no need for a long interview.

| Stable key | Skill / result | Cadence and proposed local time | Delivery | State |
|---|---|---|---|---|
| journal-morning | [Journal](skills/journal/SKILL.md): morning starter | Daily, 08:00 | Chosen morning prompt | Proposed |
| storage-report | [Storage Maintainer](skills/storage-maintainer/SKILL.md): daily changes/candidates | Daily, 18:00 | Daily concise report, even if unchanged | Proposed |
| vault-maintenance | [Vault Maintainer](skills/vault-care/SKILL.md): tags, filing, links, surfaced knowledge | Daily, 18:15 | Notify on useful findings/decision; save result each run | Proposed |
| journal-evening | [Journal](skills/journal/SKILL.md): reflection | Daily, 20:30 | Chosen evening prompt; may be skipped | Proposed |
| notion-organisation | [Notion Organizer](skills/notion-organizer/SKILL.md): selected content/navigation | Saturday, 10:00 | Findings/changes requiring attention | Proposed |
| instruction-review | [Agent Instruction Review](skills/agent-instruction-review/SKILL.md): project learnings/change proposals | Saturday, 10:30 | Private report, including no-change outcome | Proposed |
| shared-learnings | [Shared Learnings](skills/shared-learnings/SKILL.md): grouped patterns/proposals | Saturday, 11:00 | Private synthesis from available review evidence | Proposed |

If the user prefers different days/hours, their choice wins. Timing doesn't guarantee a previous
job completed: Shared Learnings must inspect the current instruction-review report and disclose
missing/stale coverage. Keep work bounded; avoid overlapping heavy local jobs. Missing connections
leave the affected routine waiting without blocking the rest of setup.

## Private reports and progress

Unless the vault schema already defines another home, use
`System/Maintenance/<stable-key>/YYYY-MM-DD.md`. Keep the source date/timezone, reviewed scope,
observed changes, evidence links, unresolved choices and next action. For a same-day retry,
read the existing report and append the new attempt/result or preserve a prior version; don't erase history.
Storage reports retain a comparable metadata baseline and identify method/coverage changes.

Expose useful findings through the chosen delivery and a link from the root README/index. Daily
storage reports are deliberately visible; other uneventful upkeep can stay quiet. Schedule/report
visibility is private by default. No automatic report pruning or retention cleanup is included.

Record native results here after activation:

| Stable key | Native task ID | Saved timing/timezone | Enabled/paused/waiting | Last attempt / last success | Report link |
|---|---|---|---|---|---|
| Add chosen job after creation | Not yet created | Not yet confirmed | Proposed | Not run | Not yet produced |

Do not call a job active until the saved task is inspected, or working until an actual result is
inspected. An offline Mac may delay local work. Use supported continuation when available; report
gaps and avoid duplicate writes. Do not invent an always-on iOS process or automatically replay
every missed run. Ask about backfill only if it would materially help.

## Approval boundaries

Scheduled maintenance may perform only the agreed housekeeping. Storage removal, moves to Trash,
backup deletion, destructive Notion reorganisation and any `AGENTS.md`/mirror edits require explicit
approval of the relevant items/actions or wording/targets. Candidate lists and grouped learnings
are proposals. Scheduling does not expand access, permit public posting or authorise paid generation.
