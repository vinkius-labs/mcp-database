# Craft.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/craftio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build product roadmaps that connect strategy to execution with visual planning tools your whole organization can follow.

## Description
Connect your **Craft.io** product management account to any AI agent and simplify how you coordinate your product strategy, manage features, and monitor roadmaps through natural conversation.

### What you can do

- **Workspace Oversight** — List all product management workspaces and retrieve detailed metadata and configurations.
- **Feature & Epic Tracking** — List, query, and create new items (features, stories, epics) within your workspaces to manage your backlog.
- **Portfolio Control** — List and query product portfolios to understand high-level organizational distribution and strategy.
- **Data Insights** — Fetch complete metadata, descriptions, and current status for any specific product item via AI.
- **Roadmap Monitoring** — Track the progress of features and epics directly from your agent to stay on top of your release cycle.
- **Operational Visibility** — Check account status and verify project metadata directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your Craft.io API Key and Account ID (found in your account settings)
3. Start managing your product ecosystem from your favorite AI assistant

### Who is this for?

- **Product Managers & Owners** — quickly retrieve feature details and update backlog items via simple AI commands.
- **Engineering Leads** — monitor epic progress and verify feature requirements directly from the workspace.
- **Product Operations** — manage workspace distributions and verify portfolio metadata via the AI assistant.


## Available Tools
- **check_craft_status**: Verify connectivity
- **create_item**: Create an item
- **get_company**: Get company details
- **get_company_competitors**: Get competitors
- **get_company_employees**: Get company employees
- **get_company_financials**: Get company financials
- **get_item**: Get item details
- **get_company_news**: Get company news
- **get_portfolio**: Get portfolio details
- **list_items**: List workspace items
- **list_portfolios**: List portfolios
- **list_workspaces**: List workspaces
- **search_companies**: Search companies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Craft.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active workspaces in my Craft.io account."

**🤖 AI Agent:**
> I've retrieved your workspaces. You have 3 active environments: 'Mobile App Roadmap', 'Web Platform Backend', and 'Design System'. Which one would you like to see items for?

---

**👤 You:**
> "Show me the last 5 items in the 'Mobile App Roadmap' (ID: 10293)."

**🤖 AI Agent:**
> I've fetched the items. For the 'Mobile App Roadmap', there are 5 recent items: 'Epic: Dark Mode Support', 'Feature: Social Login', 'Story: Fix Header Layout', and 2 others. Shall I retrieve the details for the Dark Mode epic?

---

**👤 You:**
> "Create a new feature: 'AI Search Integration' in workspace 'ws_88231'."

**🤖 AI Agent:**
> Success! The feature 'AI Search Integration' has been created in workspace ws_88231 with ID item_10293. I've added it to your product backlog in Craft.io.


## ❓ FAQ

**Q: Can I see all the items in a specific workspace via AI?**
Yes! Use the `list_workspace_items` tool and provide the Workspace ID. Your agent will retrieve all features, stories, and epics organized within that environment.

**Q: How do I add a new feature to my backlog using the agent?**
Use the `create_product_item` action. Provide the Workspace ID and the title of the feature. The agent will instantly create the record in your Craft.io account.

**Q: Is it possible to list all my product portfolios via AI?**
Absolutely. Use the `list_product_portfolios` query. The agent will retrieve the complete list of portfolios configured in your account, allowing you to monitor high-level strategy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/craftio](https://vinkius.com/mcp/craftio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Craft.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `craftio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Craft.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "craftio": {
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
