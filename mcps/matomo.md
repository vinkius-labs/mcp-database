# Matomo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/matomo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Open-source web analytics via Matomo — track visits, goals, and user behavior directly from any AI agent.

## Description
Connect your **Matomo** analytics instance to any AI agent and gain deep insights into your website traffic through natural conversation.

### What you can do

- **Visits Summary** — Get aggregated metrics on visits, actions, and bounce rates
- **Real-time Monitoring** — See the latest visitor details and actions as they happen
- **Top Content** — Identify your most visited pages, referring websites, and social networks
- **Visitor Profiles** — Inspect complete history and behavior for specific visitor IDs
- **Goal Tracking** — List and monitor conversion goals configured in your instance

### How it works

1. Subscribe to this server
2. Enter your Matomo URL, Token Auth, and Site ID
3. Start querying your web analytics from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_goals**: Get the list of goals
- **get_live_last_visits**: Get last visits in real-time
- **get_site_details**: Get details for a specific website
- **get_top_pages**: Get the most visited pages
- **get_top_referrers**: Get the top referrer types
- **get_top_socials**: Get the top referring social networks
- **get_top_websites**: Get the top referring websites
- **get_visitor_profile**: Get a detailed profile for a visitor
- **get_visits_summary**: Get a summary of visits
- **list_sites**: List all websites in Matomo


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Matomo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a summary of visits for today."

**🤖 AI Agent:**
> Retrieving summary... Today you had 1,250 visits with an average of 3 actions per visit.

---

**👤 You:**
> "What are the top pages on my site this week?"

**🤖 AI Agent:**
> Fetching top pages... The Home page and the Pricing page are your most visited content this week.

---

**👤 You:**
> "List all sites configured in Matomo."

**🤖 AI Agent:**
> Querying sites... I found 3 sites: 'E-commerce Shop', 'Blog', and 'Support Portal'.


## ❓ FAQ

**Q: How do I find my Matomo token_auth?**
Log in to Matomo, go to Personal > Security, and find the 'Auth tokens' section to generate or copy your token.

**Q: Can I track multiple sites?**
Yes, but this integration currently requires a specific Site ID. You can list all sites using the `list_sites` tool to find the correct ID.

**Q: Is my analytics data secure?**
Absolutely. Your token_auth is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/matomo](https://vinkius.com/mcp/matomo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Matomo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `matomo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Matomo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "matomo": {
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
