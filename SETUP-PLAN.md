# Set up SuperDot

Version: 1.2.0 · 2026-10-31

Work through these steps with the person. Use what they already have. Ask one small question at a
time only when a needed choice is missing. Keep credentials out of conversation. Their instructions
and existing authorisations take priority over default workflow suggestions.

## 1. Create the personal foundations

Use the connected Mac and a user-chosen folder outside this source repository. A suggested new
location is `Documents/My-SuperDot`; confirm before creating it. For an existing vault, read first
and add only missing material or an agreed narrow merge. Never replace personal files wholesale.

Copy the four files from [templates/vault](templates/vault/README.md) into the workspace root.
Create `Inbox/`, `Sources/`, `Journal/`, `Life/` and `System/`. Copy the six folders in
`templates/life/` into `Life/`. Copy the journal and project starters into `System/Templates/Journal/`
and `System/Templates/Project/`; include empty `notes/` and `assets/` folders in the project starter.

```text
My-SuperDot/
  README.md  AGENTS.md  index.md  SCHEMA.md
  Inbox/
  Sources/
  Journal/
  Life/
    Personal/  Family/  Work/  Hobbies/  Money/  Wellbeing/
  System/
    Templates/
      Journal/   # morning.md and evening.md
      Project/   # README.md, AGENTS.md, PROJECT.md, notes/, assets/
```

Open the folder in Obsidian using [the short guide](tools/obsidian.md). Obsidian is the friendly
viewer/editor; Markdown remains usable without it. If Mac access is unavailable, continue with
choices and available cloud work; say clearly that local setup has not happened yet.

## 2. Make it theirs

Read the new root `AGENTS.md`, `README.md` and `SCHEMA.md`. Fill the README's marked preferences
from known facts, then ask for missing essentials such as name and timezone. Leave optional choices
unset. Explain that any life-area name or default can be changed later; update links when renaming.

Default to concise, practical help and the six supplied areas. Projects live inside the relevant
area only when useful. The template is mostly written already; the person supplies their details.

Keep one simple checklist under “Setup progress” in their root README. Update it after useful
results or when pausing. It is enough to write `done`, `next` or `waiting` with a short reason.
Resume from that list; do not repeat finished steps or reset personal changes.

## 3. Make the skills available

Keep the complete SuperDot directory together: skill links point to shared templates, references
and notices in this package. Copying an individual skill folder alone does not include those resources.
Use the [macOS and writing standard](references/README.md#macos-and-skill-writing-standard) for local
execution; resolve the person's actual paths and tools rather than importing VPS configuration.

Use [the catalog](catalog/README.md) to choose the relevant skill and explicitly read its `SKILL.md`.
These are focused instructions for the user's Dot/local tasks, not separate running agents.
Only load what the current request needs. Add the reviewed skills through the supported local
skill/plugin mechanism if available; follow the current [official skill guide](https://developers.openai.com/plugins/build/skills).
Do not guess a Dot install command or claim the link installed anything. If installation is unavailable,
explicit file-reading is the rehearsal route; persistent automatic skill discovery remains unproven.

Introduce Note It, journal, Ponytail and i-have-adhd; let the person choose communication preferences.
Other skills are available when useful. Requesting ADHD-friendly output does not imply a diagnosis.

## 4. Remember something and reflect

Use [Note It](skills/note-it/SKILL.md) for one harmless user-chosen fact. File it in the right area,
inspect it and retrieve it. Invite a correction and preserve the correction.
Use [Journal](skills/journal/SKILL.md) to create a first entry from permitted material.

Offer morning/evening prompts, daily planning and vault care at chosen times. Save routines using
available native task features, with the user's timezone and notification choice. Record the actual
task reference in the README; if no scheduling feature is available, leave the routine on request.

## 5. Connect useful tools

Offer these setup guides, allowing each to be skipped or resumed:

- [Apple Keychain/private sign-in](tools/apple-keychain.md) for safe credential handling.
- [Notion](tools/notion.md) for selected notes, content and sharing.
- [Hosting](tools/hosting.md): choose/reuse Cloudflare or Vercel.
- [Web research](tools/web-research.md): choose/reuse Tavily or Firecrawl.
- [Hyperframes](tools/hyperframes.md) for video and presentations on the Mac.
- [ClickUp, n8n and Higgsfield](tools/planning-automation-content.md) for planning, social-media
  automations and premium content generation.

Use supported account connections and user-controlled sign-in. Email/calendar can enrich planning
and the journal after separate opt-in; other services follow as actual access becomes available.

## Finish or pause

Show the useful files/results, update the personal README checklist and name the next unfinished
step. When the Mac is offline, use a supported durable native task if available and inspect it before
calling work queued. Otherwise explain the retry needed. Before retrying a capture, inspect whether
it already saved. No extra queue software is required.

For an event demonstration, follow [the short walkthrough](checks/README.md). A written package is
ready for rehearsal; only an actual Dot run proves its discovery, permissions and execution behaviour.
