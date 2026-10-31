---
name: skill-creator
description: Create or improve a reusable skill when the user wants to preserve a useful method, using the host's supported skill-authoring tools.
license: proprietary-internal / no external licence granted
metadata:
  version: 1.0.0
  updated: 2026-10-31
  provenance: altior-authored
---

# Skill creator

Prefer a useful existing skill over another copy. Read the relevant method and what happened when
it was used. If the method is theoretical, label that clearly; don't describe it as proven.
Follow the host's supported creator and current [official skill guidance](https://developers.openai.com/plugins/build/skills).
Any applicable authoring/approval rules still apply; writing a file grants no installation authority.

For one recognisable user goal, create a lowercase kebab-case folder containing `SKILL.md` with
matching `name` and a concise `description` explaining when it applies. Record version, provenance
and licence. The body needs the useful steps, required inputs/access, output, boundaries and what
to do when something is missing. Put large detail behind relevant links only when needed.

Keep instructions portable and concise. Reuse tools; add scripts only for a concrete need. Never
embed credentials, personal records or someone else's private policies. Preserve licence notices
for adapted material and avoid invented runtime capabilities.

Inspect metadata, links and an example use appropriate to the change. Use
[skill vetting](../skill-vetting/SKILL.md) before installing unfamiliar code or permissions. Report
written versus installed versus exercised separately. Respect existing user edits on updates.
