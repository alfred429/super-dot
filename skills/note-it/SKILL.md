---
name: note-it
description: Save useful conversation content to the personal vault when asked to note it, remember this or capture an idea; also retrieve or correct a capture.
license: proprietary-internal / no external licence granted
compatibility: "Requires authorised access to the personal Markdown vault; local vault operations use the connected macOS computer."
metadata:
  target-platform: macOS
  version: "1.2.0"
  updated: "2026-10-31"
  provenance: altior-authored
---

# Note It

## Inputs and context

Use when the person asks to save, retrieve or correct useful knowledge. Identify their selected
vault, the relevant conversation/material and any existing note. Read the vault's root instructions,
preferences, schema and the applicable life-area context. For local work, follow the [macOS guidance](../../references/README.md#macos-and-skill-writing-standard).
The [starter schema](../../templates/vault/SCHEMA.md) is a reference; the person's existing schema
and personal choices govern their installed vault.

## Workflow

1. Extract the fact, idea or decision they want kept. Preserve meaning and attribution; ask only
   when missing information would materially change the content or destination.
2. Choose the relevant area or Inbox. Search existing notes and the original capture ID before
   creating another. Use the user's renamed areas when applicable; link cross-area knowledge.
3. Create or narrowly update the note with source/date, a stable capture ID and useful tags.
   Keep user statements, sourced facts and assistant inference distinguishable. Preserve meaningful
   corrections and prior content rather than replacing an entire personal note.
4. Read the saved file before confirming. For retrieval, answer from the actual note; for a correction,
   update the existing item and retain a brief change record when the meaning changes.

## Result and boundaries

Return what was kept and where, or the requested retrieved information. A successful capture
exists in the private vault, not this source repository. If access is missing, report waiting and
the needed next step; call work queued only when a durable native task actually exists.
Before retrying an interrupted write, inspect the destination for the original capture.

Do not save secrets or treat remembering as permission to share, schedule or purchase.
Example: an interest in wildlife photography becomes a Hobbies note, not an equipment order.
