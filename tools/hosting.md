# Hosting — choose one route

Version: 1.0.0 · 2026-10-31

Set up or reuse **Cloudflare or Vercel**, according to the person's preference and existing accounts.
Both are options in this starter; don't create two accounts to satisfy the guide. The goal is a
simple path to useful websites, dashboards and shareable outputs.

## Account and first project

Have the person complete sign-in/account creation through supported private browser or connection
flows. Confirm the intended account and any paid choice. Reuse an existing suitable project before
creating another. Keep application files with the relevant personal project, not in the vault's source
records or this starter repository.

- **Cloudflare:** for a simple static output, follow [Pages Direct Upload](https://developers.cloudflare.com/pages/get-started/direct-upload/).
  The dashboard can upload the prepared site folder/archive without requiring Git integration.
  Upload/deploy is a publication action: establish the audience and permission before doing it.
- **Vercel:** follow [the official getting-started guide](https://vercel.com/docs/getting-started-with-vercel)
  using the supported dashboard, connection or CLI route appropriate to the project. Use existing
  framework/tooling; no database or additional backend is required for a simple page.

Create a harmless local preview first. Before any hosted preview, explain its actual access controls;
an unlisted URL is not necessarily private. After an authorised deployment, open the result and
inspect it before returning the link. Record the account/project reference and link, never tokens.

Later dashboards can use selected connected information when authorised. Publishing a vault,
family details or secret configuration is never implied by creating a hosting account. Keep the
initial result small; adding a provider integration doesn't require building a hosting platform.
