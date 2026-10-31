---
name: vault-care
description: "Maintain the vault against its schema: check tags, filing, sources, links and discoverability; surface a concise maintenance report."
license: proprietary-internal / no external licence granted
compatibility: "Requires authorised file access to the personal vault on the connected macOS computer. Recurring care uses supported native scheduling."
metadata:
  target-platform: macOS
  version: "1.3.0"
  updated: "2026-10-31"
  provenance: altior-authored
---

# Vault Maintainer

## Inputs and context

Identify the person's vault, maintenance request or saved routine and permitted scope. Read the
actual root `SCHEMA.md`, `AGENTS.md`, index, preferences and relevant area context; don't replace
their conventions with a new taxonomy. The stable package name remains `vault-care`.
Reuse existing file/search tools and the report convention in [SCHEDULE.md](../../SCHEDULE.md).
For local work, follow the [macOS guidance](../../references/README.md#macos-and-skill-writing-standard).

## Workflow

1. Review new/changed notes since the last successful pass and selected Inbox/navigation issues.
   On the first run establish a bounded baseline, not an unsolicited whole-vault rewrite.
2. Check the actual schema's required fields: meaningful title, area, useful tags, source/date and
   capture identity where applicable. Reuse existing tag spellings; flag missing evidence rather
   than inventing provenance. Avoid forcing capture fields onto instruction or navigation files.
3. Confirm each note has one working home, related links and an appropriate index/project entry
   so useful knowledge can be found. Flag orphans, unresolved links, contradictions and duplicates.
4. Make only authorised mechanical fixes and clear Inbox filing; preserve capture IDs, personal
   wording and source originals. Inspect changes and retrieve a representative changed note.
5. Save a short private report: scope/coverage, tags/filing/link fixes made, findings needing choice,
   newly surfaced knowledge with links, and the next unresolved action. Record attempted versus
   successful coverage so a partial run doesn't advance the baseline past unreviewed material.

## Result and boundaries

Return the report link and useful findings through the chosen delivery. Keep routine notifications
quiet when nothing needs attention unless the person requested every report. Ask before deletion,
bulk moves or meaning-changing merges. Never rewrite personal reflections to make tags look tidy.

Use [Scheduling](../scheduling/SKILL.md) and the person's chosen schedule; an agreed recurring
review is not permission to change the schema or root principles.
If the Mac is unavailable, defer local work through supported tasks where possible. Do not create
a daemon, add cron jobs or promise automatic reconnection behaviour that has not been observed.
