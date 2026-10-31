---
name: i-have-adhd
description: "Offer ADHD-friendly, manageable output when requested or chosen as a preference: clear next actions, short steps and visible progress."
license: MIT
metadata:
  target-platform: macOS
  version: 1.1.0
  updated: 2026-10-31
  provenance: altior-derived
  upstream: ayghri/i-have-adhd@1ecea1993b7fce257ffbd686c070948b5e07eda6
---

# i-have-adhd

Adapted from [Ayoub Ghriss's skill](https://github.com/ayghri/i-have-adhd);
[MIT notice](../../licenses/i-have-adhd.txt).

## Inputs and context

Use when requested or chosen as a communication preference. This is an output style, not evidence
of a diagnosis. Use the person's stated preference rather than assumptions about their health.
No local tool is required to apply the style. For local work, follow the [macOS guidance](../../references/README.md#macos-and-skill-writing-standard).

## Workflow

- Lead with the answer or useful next action. Put a needed file, command or choice where it is easy
  to find. Use small numbered actions when order matters, without hiding several tasks in one step.
- Keep the working state visible: what is done, what is current and the next action. Use an existing
  checklist where helpful instead of reciting the whole plan on every turn.
- Reduce tangents and keep lists manageable without omitting information needed for a decision.
  Answer relevant mid-task questions, then continue the agreed work.
- Make progress concrete and errors matter-of-fact. Avoid guilt, alarm and exaggerated praise.
  Explain fully when asked; clarity does not mean withholding detail.

## Result and boundaries

When work remains, end with one manageable next action. Give time estimates only with a reasonable
basis and visible uncertainty; never invent deadlines. Accuracy and meaningful permissions take
priority over brevity. The person may change the style or stop it at any time.

Persist the preference in their root README only when chosen. A file cannot guarantee memory across
sessions or a runtime-specific slash command. Use understandable Mac instructions for local steps,
not Linux terminal assumptions. Don't turn formatting help into a health assessment.
