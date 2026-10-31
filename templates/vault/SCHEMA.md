# A small knowledge convention

Template version: 1.1.0 · 2026-10-31

Keep sources, maintained knowledge and personal reflection distinguishable. This is inspired by
[Karpathy's LLM wiki pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f),
with familiar life areas as the front door. No specialist database is required.

## Where things go

- **Sources:** retained originals/references in `Sources/` when useful and permitted. Keep their
  origin and capture date. Correct a derived note without silently rewriting its original source.
- **Knowledge:** a useful maintained note in one `Life/<area>/` home; related areas link to it.
- **Journal:** dated activity drafts and the person's reflection in `Journal/`, linked to relevant notes.
- **Projects:** active outcomes under an area's `Projects/`; current state belongs in `PROJECT.md`.
- **Inbox:** temporary home when the area or meaning is unclear. File gently during vault care.

## A useful note

Use a readable title and filename. Include capture date/timezone, stable capture ID, area, a few tags
and source reference. Label user statements, sourced facts and assistant inference where they differ.
For updates preserve meaningful corrections/history; link to the same note instead of making a new
master. A capture ID identifies the original request and stays the same across retries.

Illustrative Note It capture, to personalise rather than treat as a fact about the user:

```markdown
# Wildlife photography interest

- Captured: 2026-10-31, Europe/London
- Capture ID: example-photography-001
- Area: Hobbies
- Tags: photography, learning
- Source: user statement in setup conversation; conversation link unavailable

The user would like to learn wildlife photography.
No equipment purchase or project has been agreed.
```

## Updates and retrieval

Before writing, look for an existing capture or related note. Read it before editing and preserve
personal wording. If someone else changed the same content, compare versions and preserve both
when meaning conflicts. Do not silently overwrite. Inspect the saved result before confirming it.

Add a source link and a small number of useful tags; avoid rigid tagging bureaucracy. Record a brief
dated change note for a material correction. Keep secrets out of all notes. More journal access
means more available context only when the person has chosen to include that source.

## Maintenance and learnings

Keep dated upkeep reports in `System/Maintenance/<routine>/` unless an existing convention applies.
Reports record coverage, evidence, changes and proposals; link useful findings from the root/area index.
Reports aren't replacement source notes and do not authorise deletion or instruction edits.

A learning note belongs in its relevant area, with source/date, the observed outcome, affected project
or instruction file and whether the lesson is a candidate or user-confirmed. Reuse existing tags and
capture identity; link supporting reports rather than copying whole chats. Cross-project summaries
retain sources and exceptions, omit unnecessary personal detail and propose any shared rule for approval.
