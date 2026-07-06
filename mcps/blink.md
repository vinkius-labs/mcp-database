# BL.INK MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blink)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage enterprise links via BL.INK — shorten URLs, track analytics, and manage branded domains directly from any AI agent.

## Description
Connect your **BL.INK** account to any AI agent and orchestrate your enterprise link management and analytics workflows through natural conversation.

### What you can do

- **Link Shortening** — Instantly create branded short links for your marketing campaigns.
- **Link Management** — List, retrieve, update, and delete managed links across your domains.
- **Domain Oversight** — Access and manage your custom branded domains used for link shortening.
- **Click Analytics** — Retrieve real-time click metrics and historical performance for any Bitlink.
- **Tag Organization** — Access and list tags to maintain an organized inventory of your short links.
- **Account Insights** — Retrieve authenticated user profile information directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your BL.INK API Access Token
3. Start managing your enterprise links from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Professionals** — quickly create and track branded links without leaving their campaign tools.
- **Social Media Managers** — monitor link performance and update destination URLs straight from their workspace.
- **Growth Teams** — automate link creation and analytics tracking using natural language.


## Available Tools (10)
- **get_link**: Get details of a specific link
- **list_domains**: List all available domains
- **list_links**: List all managed links
- **list_tags**: List all link tags
- **shorten_link**: Shorten a long URL using BL.INK
- **update_link**: Update an existing link
- **delete_link**: Delete a link
- **get_account_info**: Get authenticated user account info
- **get_domain**: Get details of a specific domain
- **get_link_analytics**: Get click analytics for a specific link


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BL.INK** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Shorten this URL using BL.INK: https://vurb.vinkius.com/llms.txt"

**🤖 AI Agent:**
> I've shortened the link! Your new BL.INK short link is `bl.ink/xyz123`. The destination is pointing to your LLM documentation.

---

**👤 You:**
> "Show me the analytics for link link_99283."

**🤖 AI Agent:**
> Retrieving metrics... This link has received 1,250 clicks in the last 30 days. Most of the traffic is coming from social media platforms.

---

**👤 You:**
> "List my configured branded domains."

**🤖 AI Agent:**
> I've retrieved your domains. You have 2 active branded domains: 'go.company.com' (ID: dom_1) and 'links.brand.net' (ID: dom_2).


## ❓ FAQ

**Q: Can I use my own branded domain for shortening links?**
Yes! If you have branded domains configured in your BL.INK account, you can use the `list_domains` tool to find their IDs and pass a `domain_id` to the `shorten_link` action.

**Q: How do I check the click performance of a link?**
Simply ask the agent to `get_link_analytics` and provide the Link ID. It will retrieve the latest click data and statistics directly from BL.INK.

**Q: Can I update the destination URL of an existing link?**
Yes. Use the `update_link` action with the Link ID and provide the new `long_url`. Your Bitlink will redirect to the new destination immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blink](https://vinkius.com/mcp/blink)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BL.INK** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blink` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BL.INK** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blink": {
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
