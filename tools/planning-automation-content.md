# ClickUp, n8n and Higgsfield

Version: 1.0.0 · 2026-10-31

Add these when useful: ClickUp plans the work, Higgsfield creates premium media, and n8n connects
repeatable steps, especially social-media workflows. Reuse existing accounts and supported tools.
The rest of SuperDot remains useful without connecting all three.

## ClickUp — planning and follow-through

1. Reuse/create the person's chosen ClickUp workspace through private sign-in. Choose an existing
   suitable List before creating another. A simple personal/content List is enough; don't copy an
   enterprise hierarchy into someone's first setup.
2. Enable the supported ClickUp connection in the actual app. Where custom MCP is supported,
   [ClickUp's official server](https://developer.clickup.com/docs/connect-an-ai-assistant-to-clickups-mcp-server)
   uses `https://mcp.clickup.com/mcp` with OAuth. Don't substitute a chat-pasted API key.
3. Read the chosen List, then create one task when authorised: useful title, next action, links to
   relevant project/source notes, and a due date only if chosen. Inspect it and return the task link.

Use ClickUp as the working task/status home for work tracked there. Keep project context in the
vault's `PROJECT.md` and link to ClickUp rather than maintaining two competing checklists. Read
existing tasks before adding another; use the List's actual statuses instead of assuming names.
Daily planning and the journal can use this information within the person's chosen permissions.

## n8n — automations, especially social media

Reuse an existing n8n instance, or offer n8n Cloud for a straightforward start; let the person choose
any subscription. No new self-hosted server is required by this guide. Follow the official
[first-workflow guide](https://docs.n8n.io/try-it-out/quickstart/) and reuse a suitable workflow/template
after inspecting its actions. Authenticate nodes through n8n's supported
[credential setup](https://docs.n8n.io/credentials/); never put values in exported workflows or notes.

Start with a manually triggered workflow that prepares one draft or hands an approved asset to
the next step. Inspect its execution/result before enabling recurring runs. For social publishing,
choose the actual platform/account, authorised content, timezone and schedule. Use a supported node
such as [LinkedIn](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.linkedin/), or a
documented provider integration; verify its available actions and account permissions first.

Keep public posting disabled until the user authorises that scope. Check an existing task/post ID
before retrying a publishing step to avoid duplicate posts. Report the actual publishing result;
starting a workflow is not proof a post went live. If the destination isn't supported, retain a draft
for manual posting instead of building a custom publishing service.

## Higgsfield — premium content generation

Use [Higgsfield's web app](https://higgsfield.ai/) as the simplest starting point. The person signs in
privately and chooses the relevant paid plan/credits. Agree the brief, format, model and bounded
generation spend before creating content. Use only reference media the person is entitled to use.

Create a small first image/video, inspect the result and save the chosen output in the relevant
personal project's `assets/`, with its brief and source/reference links. A generation request or
preview is not a finished downloaded asset. Reuse [Hyperframes](hyperframes.md) for assembly,
captions or presentations when needed, rather than assuming Higgsfield must do every stage.

API automation is optional. Consult the current [official API quick start](https://open.higgsfield.ai/quick-start)
and its linked developer documentation before integrating; confirm authentication, selected model
schema, costs and completion handling. The documented REST base is `https://api.higgsfield.ai`.
Use supported private credentials; don't create a custom connector just to finish this setup guide.
Without an existing supported integration, use the web app and hand the saved asset to the workflow.

## One useful content loop

**Vault idea/research → ClickUp task → content draft in the project or Notion → Higgsfield asset →
review/authorisation → n8n workflow → actual platform result → ClickUp status and optional journal link.**

This is a pattern to configure with available integrations, not a preinstalled workflow. Begin with
one chosen channel and one useful result. Keep secrets in the tool's supported credential store,
private life-area material out of public content, and each service's native record as evidence.
