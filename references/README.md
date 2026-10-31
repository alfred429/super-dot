# Official guidance and upstream sources

Version: 1.2.0 · 2026-10-31

Read the relevant current developer docs when learning a tool. These are the short routes needed
by this package; installation/account availability still depends on the user's actual environment.

- **Dots:** [computers/apps](https://learn.chatgpt.com/docs/dots/computers-and-apps) and
  [tasks/memory](https://learn.chatgpt.com/docs/dots/tasks-and-memory). Local access, source scope,
  native recurring work and its connection requirements.
- **Skill packaging:** [OpenAI's skill guide](https://developers.openai.com/plugins/build/skills).
  Focused SKILL.md folders, resources and supported packaging; reading a repo isn't installation.
- **Knowledge:** [Obsidian vaults](https://obsidian.md/help/vault),
  [sync](https://obsidian.md/help/sync-notes) and
  [Karpathy's wiki pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f).
- **Native credentials:** [Apple Keychain guidance](https://support.apple.com/en-gb/guide/keychain-access/kyca1085/mac).
  Supported storage/access controls; no promise of a custom secret field in the Dot composer.
- **Notion:** [official MCP setup](https://developers.notion.com/guides/mcp/get-started-with-mcp).
- **Hosting:** [Cloudflare Direct Upload](https://developers.cloudflare.com/pages/get-started/direct-upload/)
  or [Vercel getting started](https://vercel.com/docs/getting-started-with-vercel).
- **Research:** [Tavily MCP](https://docs.tavily.com/documentation/mcp) or
  [Firecrawl in ChatGPT/Codex](https://docs.firecrawl.dev/integrations/chatgpt-codex).
- **Creative tools:** [Hyperframes upstream](https://github.com/heygen-com/hyperframes) and
  [CLI reference](https://github.com/heygen-com/hyperframes/blob/main/docs/packages/cli.mdx).
- **Planning:** [ClickUp's official MCP server](https://developer.clickup.com/docs/connect-an-ai-assistant-to-clickups-mcp-server).
- **Automations:** [n8n first workflow](https://docs.n8n.io/try-it-out/quickstart/),
  [credentials](https://docs.n8n.io/credentials/) and
  [LinkedIn node](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.linkedin/).
- **Premium content:** [Higgsfield](https://higgsfield.ai/) and [API quick start](https://open.higgsfield.ai/quick-start).

Pinned skill sources, adaptation notes and retained licences are in the [catalog](../catalog/README.md).
Use existing official integrations and methods before adding anything new.

## macOS and skill-writing standard

SuperDot uses the phone for conversation and the user's chosen Mac for local work. Confirm the
actual execution host and authorised workspace before a file operation. Cloud research or thinking
can proceed without Mac access; local writes cannot. Keep the connected Mac online with ChatGPT
open as described in the Dots guidance above. Do not silently switch to another computer.

- Resolve the person's actual home and selected vault path; quote paths containing spaces. Never
  copy a builder's Linux/VPS paths, account names or fleet configuration into the user's setup.
- Use tools already present on macOS and read official developer docs for unfamiliar commands.
  Respect the user's shell and macOS/BSD utility syntax; don't assume GNU flags, apt or systemd.
  Discover installed command locations rather than assuming a Homebrew prefix or changing PATH.
- Reuse native account permissions, supported private sign-in and Apple Keychain. Do not use
  sudo, alter privacy permissions, install software or add background services without clear scope.
- Inspect destinations before writing. Preserve personal edits and meaningful prior versions.
  Check for case-only filename collisions and existing sync copies before creating another note.
  When the Mac is unavailable, distinguish pending from saved; retry by inspecting the original result.

Every bundled skill follows the Skill Creator writing approach: precise `name`/`description`,
version/provenance/licence metadata, **Inputs and context**, **Workflow**, and **Result and boundaries**.
The description controls discovery; the body supplies task-specific decisions, relevant links and
observable completion. Reuse the root ten principles instead of repeating an enterprise policy.
Load this shared section for local work or skill authoring/vetting, not every conversational reply.
Keep optional supporting files proportional to the task. Written, installed and exercised are
different states; document checks alone establish neither activation nor real Dot compatibility.
