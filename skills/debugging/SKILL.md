---
name: debugging
description: Diagnose a concrete error or unexpected tool/software behaviour before making the smallest useful fix.
license: MIT
metadata:
  version: 1.0.0
  updated: 2026-10-31
  provenance: altior-derived
  upstream: obra/superpowers@2ce8aa15d05bd57213e6f746f953aafb7ded7a8b
---

# Debugging

Personal adaptation of Superpowers' systematic debugging; [MIT notice](../../licenses/superpowers.txt).
Find the cause before changing things. Keep the investigation proportional to the actual problem.

1. Read the error and relevant existing files/state. Reproduce through the smallest harmless action
   or inspect available evidence if reproduction is unavailable. Never dump secrets or full environments.
2. Check what changed and compare a working example. Consult current official developer docs for
   unfamiliar tools. Identify where expected behaviour first differs from what happened.
3. State one likely cause supported by evidence. Make the smallest reversible change that tests it;
   preserve existing error handling, personal data and unrelated work.
4. Repeat the relevant action or run a focused existing check. A meaningful new logic change needs
   a small behavioural check; a wording correction doesn't need a testing project.

If the fix fails, use the new evidence rather than stacking guesses. After repeated unsuccessful
attempts, stop and revisit the assumption before another edit. Ask for missing access or a decision
when needed. Never restart services, install tools or change permissions outside granted scope.

Report the cause, change and observed outcome briefly. Say what remains uncertain rather than
calling an untested change fixed. Use [Ponytail](../ponytail/SKILL.md) to keep the solution small.
