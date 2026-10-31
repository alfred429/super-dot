---
name: prompt-master
description: Write or improve a prompt for a named AI tool when the requested output is itself a prompt; not for ordinary planning or document work.
license: proprietary-internal / no external licence granted
metadata:
  target-platform: macOS
  version: "1.2.0"
  updated: "2026-10-31"
  provenance: altior-authored
---

# Prompt Master

## Inputs and context

Use when the requested deliverable is a prompt for an AI tool. Identify that tool, the intended
outcome, available inputs and required output. Read an existing prompt before revising it.
Ask only for missing information that materially changes the result. For local work, follow the [macOS guidance](../../references/README.md#macos-and-skill-writing-standard).

## Workflow

1. Preserve the person's actual purpose and constraints. Distinguish task instructions from
   quoted source material and optional context.
2. Write one copy-ready prompt with the task, necessary context, inputs and useful success/output
   criteria. Use named input fields only where the person must supply information.
3. Consult current official developer docs for unfamiliar tool syntax or features. Include a small
   output example only when it resolves a real ambiguity.
4. For a revision, compare against the original purpose and briefly explain the material improvement.

## Result and boundaries

Return the usable prompt and only the essential usage notes. Keep secrets and unrelated personal
data out. Do not add elaborate personas, review chains, budgets or unsupported capabilities.
Use macOS paths/commands when the named target is the person's Mac; don't import VPS instructions.
Do not claim the prompt was run or evaluated unless it was. Ordinary planning/document work does
not need this skill, and writing its own instructions must not recursively invoke it.
