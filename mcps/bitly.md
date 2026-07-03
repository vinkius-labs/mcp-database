# Bitly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bitly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Shorten and manage links via Bitly — track clicks, analyze metrics, and manage groups directly from any AI agent.

## Description
Connect your **Bitly** account to any AI agent and orchestrate your link management and analytics workflows through natural conversation.

### What you can do

- **Link Shortening** — Instantly shorten long URLs into branded or generic Bitlinks.
- **Click Analytics** — Retrieve real-time click counts and historical performance for any link.
- **Geographic Insights** — Analyze where your traffic is coming from with clicks-by-country metrics.
- **Referrer Tracking** — Identify which networks and sites are driving traffic to your links.
- **Group Oversight** — Manage your organization's groups and retrieve aggregated click data.
- **Tag Discovery** — Access and list tags used across your Bitlink inventory for better organization.

### How it works

1. Subscribe to this server
2. Enter your Bitly Generic Access Token
3. Start optimizing your links from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — quickly shorten links and check performance without leaving their posting tools.
- **Marketing Analysts** — retrieve geographic and referrer data for campaign reporting.
- **Growth Teams** — automate link creation and metric tracking using natural language.


## Available Tools (10)
- **list_groups**: List all Bitly groups
- **shorten_url**: Optionally set custom domain and title.

Shorten a URL
- **create_qr_code**: Generate a QR code for a link
- **get_bitlink**: Get link details
- **update_bitlink**: Update link title
- **get_clicks**: Get click analytics for a link
- **get_countries**: Get click analytics by country
- **get_referrers**: Get referrer analytics
- **list_bitlinks**: List links in a group
- **get_user**: Get account info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bitly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Shorten this URL: https://vurb.vinkius.com/docs/intro"

**🤖 AI Agent:**
> I've shortened the link! Your new Bitlink is `bit.ly/3VurbDocs`.

---

**👤 You:**
> "Show me the click summary for bit.ly/3VurbDocs."

**🤖 AI Agent:**
> The link bit.ly/3VurbDocs has received a total of 152 clicks since it was created.

---

**👤 You:**
> "List my Bitly groups."

**🤖 AI Agent:**
> Retrieving your groups... You have 2 groups: 'Marketing Team' (GUID: g_123) and 'Personal Links' (GUID: g_456).


## ❓ FAQ

**Q: Can I check how many people clicked my link today?**
Yes! Use the `get_link_clicks` tool with your Bitlink. Your agent will fetch the total click summary directly from the Bitly engine.

**Q: How do I see which countries my clicks are coming from?**
Simply ask the agent to `get_clicks_by_country` for a specific Bitlink. It will return a breakdown of traffic by geographic origin.

**Q: Does the integration allow me to delete a Bitlink?**
Bitlinks cannot be truly deleted via the standard API; they can only be archived or hidden. Currently, the toolset focuses on creation and monitoring (shortening links, checking metrics).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bitly](https://vinkius.com/mcp/bitly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bitly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bitly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bitly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bitly": {
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
