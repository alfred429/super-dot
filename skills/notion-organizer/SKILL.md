---
name: notion-organizer
description: Organise the user's chosen Notion pages and databases, keeping navigation, properties and content intact and reporting suggested structural changes.
license: proprietary-internal / no external licence granted
compatibility: "Requires a supported Notion connection with access to the selected pages/databases. Local report storage requires connected macOS file access."
metadata:
  target-platform: macOS
  version: "1.0.0"
  updated: "2026-10-31"
  provenance: altior-authored
---

# Notion Organizer

## Inputs and context

Read the chosen workspace/pages, organisation preferences and the last successful report.
Use the existing [Notion connection](../../tools/notion.md), actual page IDs and database properties.
An account connection does not put the whole workspace in scope. For local reports follow the
[macOS guidance](../../references/README.md#macos-and-skill-writing-standard).

## Workflow

1. Review the selected new/changed pages, parent structure, navigation and relevant database views.
   Establish a small baseline if no prior report exists; record access gaps.
2. Check meaningful titles, existing tags/status properties, parent placement, useful links and
   obvious duplicate/stale drafts. Use the person's current vocabulary; don't invent new databases.
3. Apply only agreed non-destructive housekeeping, such as a missing navigation link or a clearly
   established tag. Read the latest page before editing and preserve blocks, children, attachments,
   existing properties and personal changes. Use supported patch operations instead of replacing pages.
4. Propose structural moves, property/schema changes, duplicate merges, archiving or deletion with
   affected page links and reasons. Don't perform them without explicit approval for that scope.
5. Inspect each changed page and its navigation. Save a private report using
   [SCHEDULE.md](../../SCHEDULE.md): coverage, changes, unresolved findings and proposed decisions.

## Result and boundaries

Return the report and relevant page links. Maintain the chosen Notion organisation without
changing sharing permissions, publishing content or importing the private vault wholesale.
Do not treat an inaccessible page as deleted or infer that a broken lookup means a bad link.
If the connection expires or an edit conflicts, stop that action and preserve current content.
Scheduled housekeeping uses [Scheduling](../scheduling/SKILL.md); no custom Notion sync service
is required. Notion keeps its chosen published/collaborative objects; the vault remains its own home.
