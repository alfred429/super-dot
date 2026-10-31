---
name: agent-instruction-review
description: Review project AGENTS.md files against observed work, capture supported learnings in the vault and propose instruction changes for approval.
license: proprietary-internal / no external licence granted
compatibility: "Requires access to chosen project instructions, permitted work evidence and the personal vault. Local files use the connected macOS computer."
metadata:
  target-platform: macOS
  version: "1.0.0"
  updated: "2026-10-31"
  provenance: altior-authored
---

# Agent Instruction Review

## Inputs and context

Identify the approved project folders and relevant work since the last successful review. Read the
root/area/project instruction hierarchy, current project state and permitted evidence. Discover
actual `AGENTS.md` files; recognise existing `agent.md` or client mirrors without silently renaming
them or creating new copies. Follow the [macOS guidance](../../references/README.md#macos-and-skill-writing-standard).

## Workflow

1. Inventory the in-scope instruction files and their ownership. Compare instructions with actual
   completed work, explicit corrections, repeated failures and successful reusable methods.
   Use accessible project notes/results; don't assume access to all chats or read credential logs.
2. Identify stale commands, broken context pointers, duplicated/conflicting rules and useful
   missing guidance. Distinguish an instruction defect from missing access or an untested hypothesis.
3. Capture the smallest supported learning through [Note It](../note-it/SKILL.md), following the
   actual vault schema. Record source/date, affected project/file, observed outcome and candidate
   versus user-confirmed status. Search existing learnings before adding a duplicate.
4. Save a private report under [SCHEDULE.md](../../SCHEDULE.md): reviewed scope, observations,
   learning links and any proposed instruction changes. For each proposal show target file/section,
   exact before/after wording, reason, affected scope and any conflict with parent instructions.
5. Flag potentially reusable lessons for [Shared Learnings](../shared-learnings/SKILL.md).
   This is a handoff between workflows, not permission to spawn agents or copy private context.

## Result and boundaries

Surface the report even when no instruction change is recommended. Capturing a learning is not
approval to apply it. Do not edit an `AGENTS.md`, a client mirror, the root principles or another
project's instructions without explicit approval covering the proposed wording and targets.
Preserve project-specific rules and personal edits; if a proposed change conflicts with an owner
rule, report the conflict rather than weakening it. This skill reviews and proposes; it doesn't
activate skills, change account permissions or send findings outside the chosen private destination.
