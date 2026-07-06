# Xiaoshouyi / Neocrm MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/xiaoshouyi-neocrm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

China's leading enterprise CRM platform — manage leads, accounts, and opportunities via AI.

## Description
Empower your AI agent to orchestrate your sales cycle with **Xiaoshouyi** (Neocrm), the premier enterprise CRM platform in China. By connecting Xiaoshouyi to your agent, you transform complex pipeline management and customer tracking into a natural conversation. Your agent can instantly list your leads, retrieve account details, manage sales opportunities, and even audit team tasks without you needing to navigate the comprehensive web interface. Whether you are managing a large-scale sales team or a specific high-value deal, your agent acts as a real-time sales assistant, keeping your CRM data accurate and your pipeline moving.

### What you can do

- **Lead Management** — List all active leads, get detailed information, and create new prospects instantly.
- **Account & Contact Tracking** — Browse companies and individual contacts to maintain a clear picture of your customer base.
- **Opportunity Control** — Monitor sales pipelines and create new opportunities to track your deal flow effectively.
- **Task Operations** — Manage CRM tasks and activities to keep your sales team productive and aligned.
- **Sales Insights** — Retrieve high-level summaries of CRM activity and team performance.

### How it works

1. Subscribe to this server
2. Enter your Xiaoshouyi Client ID and Client Secret
3. Start managing your CRM through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — track team performance, audit pipelines, and monitor deal progress through natural language.
- **Account Executives** — manage leads and update account details directly from your AI-powered workspace.
- **Business Analysts** — retrieve CRM data for market analysis and sales forecasting through a unified AI interface.
- **Enterprise Leaders** — get real-time insights into organization-wide sales activity and customer engagement.


## Available Tools (9)
- **list_tasks**: List CRM tasks
- **list_users**: List organization users
- **create_lead**: Create a new lead
- **create_opportunity**: Create a new opportunity
- **get_lead**: Get lead details
- **list_accounts**: List CRM accounts
- **list_contacts**: List CRM contacts
- **list_leads**: List CRM leads
- **list_opportunities**: List sales opportunities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Xiaoshouyi / Neocrm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active leads from Xiaoshouyi."

**🤖 AI Agent:**
> I've retrieved your active leads. You have 120 leads in total, including 15 new ones from today. Would you like to see the details of the most recent ones?

---

**👤 You:**
> "Create a new opportunity for account 'Tech Giant' titled 'Enterprise License Renewal'."

**🤖 AI Agent:**
> Done! I've created the opportunity 'Enterprise License Renewal' for the 'Tech Giant' account. I've set it to the 'Initial Contact' stage by default. Would you like to add an expected amount?

---

**👤 You:**
> "Show me a summary of my CRM activity for this week."

**🤖 AI Agent:**
> I've retrieved your CRM summary. This week, you've engaged with 45 leads, opened 8 new opportunities, and completed 12 tasks. Your pipeline health is currently stable. Would you like a breakdown by project?


## ❓ FAQ

**Q: How do I find my Xiaoshouyi Client ID and Secret?**
Log in to the Xiaoshouyi administration console, go to [PaaS Platform] → [App Management], and create a new application to generate your Client ID and Client Secret.

**Q: Can I filter leads by specific criteria?**
Yes. When using the `list_leads` tool, you can provide an optional `filter` parameter to narrow down the results based on status, source, or other CRM fields.

**Q: Is it possible to create tasks for my team?**
Yes, while the current tools focus on listing tasks, you can use the AI agent to coordinate assignments and update existing task statuses through the CRM's unified interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/xiaoshouyi-neocrm](https://vinkius.com/mcp/xiaoshouyi-neocrm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Xiaoshouyi / Neocrm** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `xiaoshouyi-neocrm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Xiaoshouyi / Neocrm** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "xiaoshouyi-neocrm": {
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
