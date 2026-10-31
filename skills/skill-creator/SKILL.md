---
name: skill-creator
description: Create or improve a reusable skill when the user wants to preserve a useful method, using the host's supported skill-authoring tools.
license: proprietary-internal / no external licence granted
metadata:
  target-platform: macOS
  version: "1.2.0"
  updated: "2026-10-31"
  provenance: altior-authored
---

# Skill creator

## Inputs and context

Identify the requested user goal, existing method, intended runtime and any skill being changed.
Check for an adequate existing skill first. Prefer a method supported by real usage; label an
untested method honestly. Read the [shared writing/macOS standard](../../references/README.md#macos-and-skill-writing-standard)
and the cross-company [Agent Skills specification](https://agentskills.io/specification).
Use the host's [product guidance](https://developers.openai.com/plugins/build/skills) for installation.

## Workflow

1. Use the supported creator where available and respect the requested output location. Updating
   an existing skill does not require reinitialising its directory or installing it.
2. Give one recognisable purpose a lowercase kebab-case folder and matching `name`. Write a concise
   discovery `description`. Keep version/provenance in `metadata` as string values, including quoted
   dates. Retain licences/notices; use optional `compatibility` only for actual environment requirements.
3. State relevant inputs/access, the useful workflow, observable result and what to do when access
   or authority is missing. Keep detailed material in supporting files only when it earns its place.
4. Tailor machine-specific guidance to macOS. Avoid builder-specific home paths, GNU-only command
   assumptions, Linux service managers and hidden dependencies on private company configuration.
5. Inspect frontmatter, references and a representative use appropriate to the change. Use the
   host creator's lightweight validator when available; don't install a testing stack for a text edit.

## Result and boundaries

Return the skill location, purpose and what was checked. Distinguish written, installed and
exercised. Follow any applicable authoring/approval rules; file creation grants no runtime permission.
Use [skill vetting](../skill-vetting/SKILL.md) for unfamiliar code or permissions before adoption.

Never embed credentials or personal records. Reuse tools, preserve user edits and avoid extra
scripts, UI metadata, manifests or auxiliary docs unless the actual packaging/workflow needs them.
