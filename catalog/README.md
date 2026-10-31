# SuperDot capability catalog

Version: 1.1.0 · 2026-10-31

One personal starter repository. The Markdown supplies guidance and reusable foundations;
skills use the tools and permissions actually available in the user's environment.

## Included skills

| Skill | What it helps with |
|---|---|
| [Note It](../skills/note-it/SKILL.md) | Capture, retrieve and correct useful knowledge. |
| [Journal](../skills/journal/SKILL.md) | Morning/evening reflection that grows with chosen sources. |
| [Vault care](../skills/vault-care/SKILL.md) | Gentle filing, links and maintenance. |
| [Brainstorming](../skills/brainstorming/SKILL.md) | Explore options and choose a useful experiment. |
| [Grill Me](../skills/grill-me/SKILL.md) | Challenge an idea when explicitly requested. |
| [Prompt Master](../skills/prompt-master/SKILL.md) | Produce a prompt for the named AI tool. |
| [Debugging](../skills/debugging/SKILL.md) | Find the cause and make a small verified fix. |
| [Skill creator](../skills/skill-creator/SKILL.md) | Capture a useful reusable method. |
| [Skill vetting](../skills/skill-vetting/SKILL.md) | Inspect additions before adoption. |
| [Ponytail](../skills/ponytail/SKILL.md) | Reuse and the smallest complete solution. |
| [i-have-adhd](../skills/i-have-adhd/SKILL.md) | Manageable, actionable output when chosen. |
| [Research](../skills/research/SKILL.md) | Search/extract, inspect sources and retain useful findings. |
| [Daily planning](../skills/daily-planning/SKILL.md) | Priorities, commitments and user-chosen routines. |

## Foundations and choices

| Module | Default / choice | Needs |
|---|---|---|
| Personal vault | Obsidian-compatible Markdown; six life areas | Private user-owned location; Mac access for local writes |
| Project starters | Ready README, AGENTS and PROJECT files | Actual user goal and a few personal edits |
| Journal | Selected conversation material first | Separate opt-in for each additional source |
| Routines | On request until times chosen | Supported native schedules, timezone and notification destination |
| Credential custody | Apple Keychain and supported private sign-in | Tool-specific private authentication/use; generic custom entry unproven |
| Notes/content/sharing | Notion | Chosen account, destination and sharing scope |
| Hosting | Cloudflare **or** Vercel | One reused/new account; publication and costs chosen by user |
| Search/extraction | Tavily **or** Firecrawl | One supported connection; bounded usage |
| Creative outputs | Hyperframes | Existing/supported Mac installation and its upstream skills |
| Planning | [ClickUp](../tools/planning-automation-content.md) | Chosen workspace/List and supported connection; one working task/status home |
| Social-media automations | [n8n](../tools/planning-automation-content.md) | Existing instance or chosen Cloud account, supported nodes and authorised publishing scope |
| Premium media | [Higgsfield](../tools/planning-automation-content.md) | Chosen account/credits, generation brief and supported web/API route |

Use [tool guides](../tools/obsidian.md) and [setup](../SETUP-PLAN.md) for the actual steps.
Local skills need a connected computer under current Dots guidance. File instructions can be read
explicitly; automatic discovery/installation still depends on the runtime. No account is connected
merely by including its guide. There is no Supabase dependency.

## Upstream revisions and notices

Reviewed 2026-10-31; these pins identify the inspected sources, not a floating update subscription.

| Upstream | Inspected revision | Used here | Licence |
|---|---|---|---|
| [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail/tree/96608e078b2d5ea607c5c3b8b5a54d1c1fba6846) | `96608e078b2d5ea607c5c3b8b5a54d1c1fba6846` | Portable metadata/level selection; core method retained | [MIT notice](../licenses/ponytail.txt) |
| [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd/tree/1ecea1993b7fce257ffbd686c070948b5e07eda6) | `1ecea1993b7fce257ffbd686c070948b5e07eda6` | Personal output adaptation; no diagnosis, unsupported flags or invented time estimates | [MIT notice](../licenses/i-have-adhd.txt) |
| [obra/superpowers](https://github.com/obra/superpowers/tree/2ce8aa15d05bd57213e6f746f953aafb7ded7a8b) | `2ce8aa15d05bd57213e6f746f953aafb7ded7a8b` | Simplified brainstorming and debugging; no mandatory review/delegation chain | [MIT notice](../licenses/superpowers.txt) |

Remaining skills and personal templates are original SuperDot material. No external licence is
granted for that original material in this build; this is separate from the retained upstream MIT
licences. Publishing/relicensing the original package is an owner decision.

Karpathy's [LLM wiki pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)
is a conceptual reference for source-backed maintained knowledge; its text is not bundled.
Connected services and Hyperframes are external tools, not vendored software. Resolve their current
supported version/setup from official docs and record actual installed versions in the personal README
when useful. Do not automatically execute remote installers from a catalog entry.
