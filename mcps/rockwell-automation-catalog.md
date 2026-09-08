# Rockwell Automation Catalog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rockwell-automation-catalog)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Rockwell Automation Experience (X) APIs as an MCP: universal search across the product catalog (ControlLogix, PowerFlex, PanelView...) and the partner directory (System Integrators, distributors) — api.rockwellautomation.com with OAuth2 client auth.

## Description
**Rockwell Automation Experience (X) APIs** — the official API gateway of Rockwell Automation (api.rockwellautomation.com, Anypoint) as a single MCP server.

### What you can do
- **Universal catalog search** — search Rockwell's full product universe: ControlLogix controllers, PowerFlex drives, PanelView HMIs, Guardmaster safety, part numbers, downloads and documentation in one query
- **Partner directory** — browse System Integrators, distributors and OEMs by program tier (SI Gold, Distributor...) from the official partner database

### Authentication
1. Register your application for the Rockwell Experience APIs (FactoryTalk / X API program)
2. Copy the issued **Client ID + Client Secret** into this MCP's credentials
3. The gateway validates OAuth 2.0 client credentials server-side on every call (sent as HTTP Basic); unauthenticated calls return `{"error": "Invalid client id or secret"}`

### Who is this for?
Control systems engineers, panel builders, distributors, purchasing/procurement tools and AI agents that need authoritative Rockwell product and partner data.


## Available Tools (2)
- **list_partners**: ), descriptions and facets. Pagination via startIndex/numResults. Requires the Partners product on your Experience API app.

List Rockwell Automation partner companies (System Integrators, distributors) with program tiers
- **search_catalog**: Returns matched products (part numbers, descriptions), downloads and documentation. Pagination via from + size counts. Requires an approved Rockwell Experience API app; 401 "Invalid client id or secret" means the key/secret pair is wrong or the app lacks approval.

Search the Rockwell Automation product catalog: ControlLogix, PowerFlex, PanelView part numbers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rockwell Automation Catalog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the ControlLogix 1756-L83E controller and its documentation"

**🤖 AI Agent:**
> 🏭 **Catalog search: 1756-L83E (Rockwell Experience API)**

Products:
- 1756-L83E — ControlLogix 5580 controller, 40MB user memory
Downloads: firmware release notes, AOPs
Documents: installation instructions, user manuals

Want matched downloads (firmware versions) or sibling controllers (1756-L82, -L84)?

---

**👤 You:**
> "Find a Gold-level System Integrator partner near me"

**🤖 AI Agent:**
> 🤝 **Rockwell partner directory (SI Gold tier)**

Partners found via the /partners API with program type SI Gold — certified integrators for Logix-based systems.

Each entry includes description and program tier from the official partner database. Want the full list or filtered by region?

---

**👤 You:**
> "Search for PowerFlex 525 drive downloads"

**🤖 AI Agent:**
> 📦 **PowerFlex 525 — downloads section**

From the universal search: firmware releases, AOP (Add-On Profiles), connected component workbench files and documentation — with size counts per section.

Want product specs instead, or matching 25A-525 part numbers?


## ❓ FAQ

**Q: How do I get the Client ID/Secret?**
Register your application for the Rockwell Experience APIs (via the Rockwell Automation Developer program / FactoryTalk Hub). After approval you receive a client key (ID) and secret pair that this MCP sends as HTTP Basic credentials on every gateway call.

**Q: I get 'Invalid client id or secret' — what does it mean?**
The gateway's OAuth 2.0 policy rejected your credentials: either the key/secret pair is wrong, or your app registration isn't approved/active for the requested product. Verify both in your Rockwell Developer account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rockwell-automation-catalog](https://vinkius.com/ai-agent-connect/rockwell-automation-catalog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rockwell Automation Catalog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rockwell-automation-catalog` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rockwell Automation Catalog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rockwell-automation-catalog": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
