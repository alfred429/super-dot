---
name: storage-maintainer
description: Produce a daily macOS storage-change report and a clear cleanup candidate list; never delete or move anything without explicit approval.
license: proprietary-internal / no external licence granted
compatibility: "Requires read access to approved Mac folders and native disk/file metadata. Reports use a private writable destination; no extra scanner is required."
metadata:
  target-platform: macOS
  version: "1.0.0"
  updated: "2026-10-31"
  provenance: altior-authored
---

# Storage Maintainer

## Inputs and context

Identify the intended Mac, volume, approved folders, report destination and previous comparable
report. Follow the [macOS guidance](../../references/README.md#macos-and-skill-writing-standard).
Measure metadata with existing native tools; don't install a scanner, read file contents or scan
the whole home by default. Exclude secret stores, protected system areas and unapproved folders.

## Workflow

1. Record observation time/timezone, host, disk method, free/available figures and folder coverage.
   Treat macOS available/purgeable space and allocated file sizes as different measurements;
   use consistent units/methods and don't promise that candidate sizes equal reclaimable space.
2. Within approved folders, compare bounded path/size/modified-time inventories to the previous
   successful comparable report. Surface new items, growth and items no longer observed. A missing
   path may have moved or become inaccessible; don't label it deleted without evidence.
3. On the first run report a baseline, with changes unknown. For partial coverage, identify gaps;
   don't invent a change total or silently compare different scopes/methods.
4. List useful cleanup candidates with exact private path, measured size, last modification,
   likely purpose, reason, dependencies/uncertainty and suggested action. Preserve active project
   assets, backups and source records. Age or a cache-like name alone is not proof something is disposable.
5. Save a dated daily report under the private report convention in [SCHEDULE.md](../../SCHEDULE.md).
   Include disk summary, largest relevant changes, candidates and an explicit “Nothing removed” line.
   Keep prior reports/baselines; no automatic pruning or cleanup of the reports themselves.

## Result and boundaries

Deliver the daily report, including an unchanged result, through the chosen channel. Example:
“No comparable baseline yet; these are current sizes, not today's growth.” Never export private
filenames to a public dashboard. Report storage permissions as a limit; don't use sudo or expand access.

This skill reports and recommends. Deleting, emptying Trash, moving to Trash, relocating files,
purging caches or overwriting backups requires explicit approval naming the items and action;
a schedule or “keep storage tidy” is not that approval. Recheck approved items for changes and
dependencies immediately before acting, use a recoverable route where possible, then inspect the
result. Do not turn a candidate report into automatic cleanup. Use [Scheduling](../scheduling/SKILL.md)
for native daily reporting, not a background disk-monitoring service.
