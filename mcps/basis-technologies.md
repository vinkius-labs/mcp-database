# Basis Technologies MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/basis-technologies)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your Basis DSP campaigns, tactics, and ads directly from any AI agent.

## Description
Connect your **Basis Technologies (formerly Centro)** account to any AI agent and orchestrate your programmatic advertising workflows through natural conversation.

### What you can do

- **Campaign Management** — List all media buying campaigns and fetch detailed metadata from the Basis cloud.
- **Tactic Optimization** — Query and inspect specific tactics (line items) to understand targeting, pacing, and bidding strategies.
- **Ad Creative Audit** — List all ad creatives and verify statuses across your digital advertising portfolio.
- **Performance Analytics** — Retrieve real-time delivery statistics and KPIs for campaigns and tactics to drive data-informed decisions.
- **Client & Brand Oversight** — Maintain a clear view of all advertisers and brands managed within your organization.

### How it works

1. Subscribe to this server
2. Enter your Basis DSP Access Token
3. Start optimizing your ad spend from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Media Buyers & Planners** — instantly check campaign statuses and pacing without navigating complex DSP dashboards.
- **AdOps Teams** — audit ad creatives and tactic configurations straight from your workflow tools.
- **Account Managers** — retrieve performance reports for clients on the fly during meetings or via automated summaries.


## Available Tools
- **get_ad**: Get specific ad details
- **list_brands**: List all brands
- **get_campaign_performance**: Get performance metrics for a campaign
- **get_campaign**: Get specific Basis campaign details
- **get_tactic_performance**: Get performance metrics for a tactic
- **list_ads**: List all ad creatives
- **get_tactic**: Get specific Basis tactic details
- **list_campaigns**: List all Basis DSP campaigns
- **list_clients**: List all clients/advertisers
- **list_tactics**: List all Basis DSP tactics (line items)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Basis Technologies** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns in my Basis account."

**🤖 AI Agent:**
> I've retrieved 3 active campaigns: 'Summer Sale 2024' (ID: 88231), 'Retargeting Q3' (ID: 88245), and 'Brand Awareness' (ID: 88250). Which one would you like to inspect further?

---

**👤 You:**
> "Show performance stats for campaign 88231."

**🤖 AI Agent:**
> Campaign 'Summer Sale 2024' (88231) has delivered 1.2M impressions with a CTR of 0.45%. Total spend is $5,400 against a $10,000 budget. Pacing is currently on track.

---

**👤 You:**
> "List all tactics associated with my account."

**🤖 AI Agent:**
> I found 5 tactics currently configured. Notable ones include 'Audience: Home Owners' and 'Geo: New York Metro'. Would you like the full details for any of these?


## ❓ FAQ

**Q: Can I check the real-time performance of a specific campaign?**
Yes! Use the `get_campaign_performance` tool with the Campaign ID. Your agent will fetch the latest KPIs including impressions, clicks, and spend directly from the Basis analytics engine.

**Q: How do I list all active tactics for my account?**
Simply ask the agent to `list_tactics`. It will retrieve the execution-level line items, showing their status and basic configuration for your review.

**Q: Does this integration allow making changes to my budgets?**
Currently, the toolset is focused on querying and analysis (Read-Only). You can list and inspect campaigns, tactics, and performance, but budget adjustments must be performed within the Basis DSP platform for security.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/basis-technologies](https://vinkius.com/mcp/basis-technologies)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Basis Technologies** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `basis-technologies` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Basis Technologies** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "basis-technologies": {
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
