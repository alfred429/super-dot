---
name: ponytail
description: Use the smallest complete solution for coding/build tasks, especially when asked for Ponytail, simplicity, reuse or less overengineering.
license: MIT
metadata:
  target-platform: macOS
  version: "1.2.0"
  updated: "2026-10-31"
  provenance: altior-derived
  upstream: DietrichGebert/ponytail@96608e078b2d5ea607c5c3b8b5a54d1c1fba6846
---

# Ponytail

Adapted from [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail);
[MIT notice](../../licenses/ponytail.txt). The core principle is the smallest complete solution.

## Inputs and context

Read the requested outcome and the existing files/tools it touches. Identify the callers,
configuration or outputs that must remain consistent. Separate required scope from attractive extras.
For local work, follow the [macOS guidance](../../references/README.md#macos-and-skill-writing-standard). Apply for the session once requested until the user changes that preference.

## Workflow

1. Check whether the proposed mechanism needs to exist. Reuse an adequate existing workflow or
   implementation first, then native platform/standard-library capabilities, then an installed dependency.
2. If new work is necessary, make the smallest readable change that fully solves the request.
   Avoid speculative abstractions, wrappers, options, dependencies and auxiliary documentation.
3. Preserve the codebase's conventions, error handling, validation, accessibility and personal data.
   For a bug, inspect relevant callers and fix the shared cause rather than repeating a workaround.
4. Check the actual result. Use a focused existing check or one small behavioural check for meaningful
   new logic. A trivial text edit needs inspection, not a testing programme.

## Result and boundaries

Return the useful outcome and material limitation briefly. Name skipped work only when it affects
expectations. Do not report an unrun check as passed. Simplicity never permits data loss, weakened
permissions or omission of a requirement the user actually asked for.

On macOS reuse available apps/tools; don't add Linux packages, service wrappers or a custom daemon
for a solved problem. Offer levels in ordinary language: lite completes the request and mentions
a smaller alternative; full applies these defaults; ultra also questions unjustified scope.
Levels do not override the user's intent or permission boundaries.
