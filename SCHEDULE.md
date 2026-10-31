# SuperDot routines and maintenance schedule

Version: 1.1.0 · 2026-10-31 · Complete run policy: defaults ready for setup, not active tasks

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

This is the standard routine bundle. During an authorised SuperDot setup, offer it as one preset
the person can accept or change. Resolve timezone, permitted scope and private delivery from existing
preferences first; ask only for missing essentials. Programme the accepted bundle using native tasks,
not a separate approval conversation for each job. Respect any jobs already declined or paused.
Rows remain **proposed** until actual task creation/readback; the optional research job stays off
until a topic/source scope is chosen. No Dot schedules have been activated by writing this file.

| Stable key | Skill / result | Cadence and proposed local time | Delivery | State |
|---|---|---|---|---|
| journal-morning | [Daily Planning](skills/daily-planning/SKILL.md) → [Journal](skills/journal/SKILL.md): one combined priorities/commitments/morning starter | Daily, 08:00 | One morning brief, not two separate prompts | Proposed |
| storage-report | [Storage Maintainer](skills/storage-maintainer/SKILL.md): daily changes/candidates | Daily, 18:00 | Daily concise report, even if unchanged | Proposed |
| vault-maintenance | [Vault Maintainer](skills/vault-care/SKILL.md): tags, filing, links, surfaced knowledge | Daily, 18:15 | Notify on useful findings/decision; save result each run | Proposed |
| journal-evening | [Journal](skills/journal/SKILL.md): reflection | Daily, 20:30 | Chosen evening prompt; may be skipped | Proposed |
| notion-organisation | [Notion Organizer](skills/notion-organizer/SKILL.md): selected content/navigation | Saturday, 10:00 | Findings/changes requiring attention | Proposed |
| instruction-review | [Agent Instruction Review](skills/agent-instruction-review/SKILL.md): project learnings/change proposals | Saturday, 10:30 | Private report, including no-change outcome | Proposed |
| shared-learnings | [Shared Learnings](skills/shared-learnings/SKILL.md): grouped patterns/proposals | Saturday, 11:00 | Private synthesis from available review evidence | Proposed |
| schedule-review | [Scheduling](skills/scheduling/SKILL.md): compare accepted routines with saved native tasks and recent results | Saturday, 11:30 | Missing/duplicate/stale-job findings and needed decisions | Proposed |
| research-brief | [Research](skills/research/SKILL.md): one bounded chosen-topic brief; retain useful findings through Note It if chosen | Daily, 08:30, only when enabled | Chosen topic, sources and private brief destination required | Optional; off |

If the user prefers different days/hours, their choice wins. Timing doesn't guarantee a previous
job completed: Shared Learnings must inspect the current instruction-review report and disclose
missing/stale coverage. Keep work bounded; avoid overlapping heavy local jobs. Missing connections
leave the affected routine waiting without blocking the rest of setup.

## When every skill runs

Every skill has a run policy; a timer is useful only for recurring work. Event-driven means the
assistant invokes the workflow in the current task, not that a file watcher or new background
service must be installed. Existing authorisation and access boundaries still apply.

| Skill | Run policy | Trigger / schedule |
|---|---|---|
| [Note It](skills/note-it/SKILL.md) | Request/workflow-driven | “Note it”, retrieve/correct a capture, or an agreed review/research workflow retaining knowledge. |
| [Journal](skills/journal/SKILL.md) | Scheduled and on request | `journal-morning` / `journal-evening`; optional reflection whenever asked. |
| [Vault Maintainer](skills/vault-care/SKILL.md) | Scheduled and on request | `vault-maintenance`; a specific filing/tag/link request can run immediately. |
| [Brainstorming](skills/brainstorming/SKILL.md) | On request | Explore an idea or an unsettled practical choice; no automatic brainstorming job. |
| [Grill Me](skills/grill-me/SKILL.md) | Explicit request | Challenge/stress-test when invited, not as unsolicited periodic critique. |
| [Prompt Master](skills/prompt-master/SKILL.md) | On request | The requested output is a prompt for a named AI tool. |
| [Debugging](skills/debugging/SKILL.md) | Event/request-driven | A concrete error or unexpected result in authorised work; no speculative background scans. |
| [Skill creator](skills/skill-creator/SKILL.md) | On request | Preserve/improve a useful method when wanted, not a daily skill-generation quota. |
| [Skill vetting](skills/skill-vetting/SKILL.md) | Before adoption/update | Inspect an unfamiliar new or changed skill/plugin before authorised use. |
| [Ponytail](skills/ponytail/SKILL.md) | Working preference | Apply to relevant building/coding tasks once chosen; no timed execution. |
| [i-have-adhd](skills/i-have-adhd/SKILL.md) | Communication preference | Apply to replies when selected; no timed execution or inferred diagnosis. |
| [Research](skills/research/SKILL.md) | On request; optional recurring | Research questions as needed; `research-brief` only with a chosen scope. |
| [Daily Planning](skills/daily-planning/SKILL.md) | Scheduled and on request | Included in `journal-morning`; also replan when asked or commitments change. |
| [Notion Organizer](skills/notion-organizer/SKILL.md) | Scheduled and on request | `notion-organisation` for chosen connected pages; targeted tidying when requested. |
| [Storage Maintainer](skills/storage-maintainer/SKILL.md) | Daily and on request | `storage-report`; a requested check can run sooner within approved folders. |
| [Agent Instruction Review](skills/agent-instruction-review/SKILL.md) | Weekly and on request | `instruction-review`; an explicit correction/incident can warrant a focused earlier review. |
| [Shared Learnings](skills/shared-learnings/SKILL.md) | Weekly and on request | `shared-learnings` after available review reports; compare a chosen lesson when requested. |
| [Scheduling](skills/scheduling/SKILL.md) | Setup/change-driven and weekly | Programme the accepted preset during setup; `schedule-review` checks saved jobs; apply requested pauses/changes. |

Default setup therefore programmes **eight recurring jobs**, subject to available tools/access and
the person's accepted settings. Research is the ninth possible job and is optional. Do not create
timers for request-driven skills just to make every skill appear scheduled. Template timing is a
starting point, not a claim that a job has been saved or will run while its Mac is unavailable.

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
