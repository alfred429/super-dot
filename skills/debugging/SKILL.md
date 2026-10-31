---
name: debugging
description: Diagnose a concrete error or unexpected tool/software behaviour before making the smallest useful fix.
license: MIT
metadata:
  target-platform: macOS
  version: 1.1.0
  updated: 2026-10-31
  provenance: altior-derived
  upstream: obra/superpowers@2ce8aa15d05bd57213e6f746f953aafb7ded7a8b
---

# Debugging

Adapted from Superpowers' systematic debugging;
[MIT notice](../../licenses/superpowers.txt).

## Inputs and context

Identify expected versus actual behaviour, the smallest available reproduction, relevant files
and recent changes. Establish the real execution host before interpreting an error.
For local work, follow the [macOS guidance](../../references/README.md#macos-and-skill-writing-standard).

## Workflow

1. Read the error and relevant existing state. Reproduce through a harmless action or use available
   evidence when reproduction is unavailable. Never dump credentials or the full environment.
2. Compare a working example and consult official docs for unfamiliar tools. For macOS command
   failures, check the installed command, shell, permissions and BSD/GNU differences before editing
   configuration. Don't assume a missing shell command means a new install is required.
3. State one evidence-backed hypothesis and make the smallest reversible change that addresses it.
   Preserve error handling, personal data and unrelated work.
4. Repeat the relevant action or use a focused existing check. A meaningful logic change warrants
   one small behavioural check; a wording correction does not need a test programme.

## Result and boundaries

Report the cause, change and observed result. If a fix fails, use the new evidence rather than
stacking guesses. After repeated unsuccessful attempts, stop and revisit the assumption or ask
for the missing decision/access. Say unverified when the outcome cannot be checked.

Use [Ponytail](../ponytail/SKILL.md) for proportional changes. Do not restart services, install tools,
use sudo or change account/privacy permissions outside the user's granted scope.
