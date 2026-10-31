---
name: scheduling
description: Create, review or change SuperDot native routines from the user's chosen SCHEDULE.md, avoiding duplicates and verifying what was actually saved.
license: proprietary-internal / no external licence granted
compatibility: "Requires supported native scheduling tools to create routines. Local jobs also require connected macOS access; absent scheduling leaves routines on request."
metadata:
  target-platform: macOS
  version: "1.0.0"
  updated: "2026-10-31"
  provenance: altior-authored
---

# Scheduling

## Inputs and context

Read the person's private `System/SCHEDULE.md`, copied initially from the package's
[SCHEDULE.md](../../SCHEDULE.md). Their edited private copy owns their choices. Read relevant
preferences, actual tool availability and existing native schedules before changing anything.
Follow the [macOS guidance](../../references/README.md#macos-and-skill-writing-standard).

## Workflow

1. Confirm chosen jobs, local timezone, times, scope and delivery settings. Suggested template times
   are proposals, not permission to create every routine. Reuse prior clear authorisation; don't
   repeatedly ask for the same accepted settings.
2. Resolve each stable schedule key against its saved native task ID and live schedules. Reuse/update
   the matching task rather than creating duplicates. Investigate ambiguous matches before writing.
3. Create/update only chosen jobs with the available native scheduling tool. State the skill entrypoint,
   package/vault/report location, bounded scope, timezone, cadence, notification rule and approval limits.
   Paths must be accessible from the actual execution environment; don't assume a cloud task can
   open Mac files while that Mac is unavailable.
4. Read back the saved task. Record its actual ID, saved timing/timezone and enabled/paused state
   in the private schedule record. A rejected/unavailable creation remains waiting or on request.
5. Inspect the first actual output when available and record last attempted versus last successful
   run. Show stale/unavailable jobs honestly; don't claim the routine works from configuration alone.

## Result and boundaries

Report what was saved or changed and what still waits. Follow user-directed pauses/cancellations
and confirm them against native state. Stopping active work and cancelling a recurring task are
separate actions; clarify which when the request is ambiguous. Keep scheduled jobs within their
scope: reporting does not authorise deletion, instruction changes, spending or external publishing.

Use native catch-up/continuation only when supported. Don't shut down/disconnect devices to test
offline behaviour, create cron/launchd services, build a scheduler or replay a backlog automatically.
If a predecessor report is missing, dependent review reports the gap instead of inventing results.
