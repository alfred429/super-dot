# SuperDot capability catalog

Version: 1.4.0 · 2026-10-31

One personal starter repository. The Markdown supplies guidance and reusable foundations;
skills use the tools and permissions actually available in the user's environment.

All 18 skills follow the [shared macOS/writing standard](../references/README.md#macos-and-skill-writing-standard),
with precise discovery descriptions, inputs/context, workflow, completion/boundaries and versioned
provenance. Versions are recorded per skill: Vault Maintainer, Journal and Daily Planning are v1.3.0,
the five new upkeep/scheduling skills are v1.0.0, and the remaining core skills are v1.2.0. All align with the
[Agent Skills specification](https://agentskills.io/specification): string-valued custom metadata
and environment compatibility where needed. Our body headings are a house convention, not extra
required specification fields. Preserve this repository's layout when using them:
their supporting links reach shared templates/references/notices. These are repository-bundled
instructions; no custom plugin manifest or automatic Dot activation is claimed. External plugin
connections are covered by the tool guides, not reimplemented in this repo.

## Included skills

| Skill | What it helps with |
|---|---|
| [Note It](../skills/note-it/SKILL.md) | Capture, retrieve and correct useful knowledge. |
| [Journal](../skills/journal/SKILL.md) | Morning/evening reflection that grows with chosen sources. |
| [Vault Maintainer](../skills/vault-care/SKILL.md) | Schema checks, tags, filing, links, discoverability and maintenance reporting; stable name `vault-care`. |
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
| [Notion Organizer](../skills/notion-organizer/SKILL.md) | Keep chosen pages/databases organised while preserving content and sharing boundaries. |
| [Storage Maintainer](../skills/storage-maintainer/SKILL.md) | Daily storage changes and cleanup candidates; no removal without explicit approval. |
| [Agent Instruction Review](../skills/agent-instruction-review/SKILL.md) | Review project instructions, capture learnings and propose precise changes for approval. |
| [Shared Learnings](../skills/shared-learnings/SKILL.md) | Group cross-project lessons and propose where guidance belongs, without automatic propagation. |
| [Scheduling](../skills/scheduling/SKILL.md) | Create/reuse native routines from the person's chosen schedule and inspect saved state/results. |

## Foundations and choices

| Module | Default / choice | Needs |
|---|---|---|
| Personal vault | Obsidian-compatible Markdown; six life areas | Private user-owned location; Mac access for local writes |
| Project starters | Ready README, AGENTS and PROJECT files | Actual user goal and a few personal edits |
| Journal | Selected conversation material first | Separate opt-in for each additional source |
| Routines | [SCHEDULE.md](../SCHEDULE.md) supplies editable proposals | Chosen jobs/scope, timezone, delivery and supported native scheduling; no automatic activation |
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
| [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail/tree/96608e078b2d5ea607c5c3b8b5a54d1c1fba6846) | `96608e078b2d5ea607c5c3b8b5a54d1c1fba6846` | Concise professional/macOS adaptation; core reuse/smallest-complete-solution method retained | [MIT notice](../licenses/ponytail.txt) |
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
