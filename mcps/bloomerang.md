# Bloomerang MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bloomerang)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage donors and donations via Bloomerang — list constituents, transactions, and campaigns directly from any AI agent.

## Description
Connect your **Bloomerang** donor management system to any AI agent and orchestrate your non-profit fundraising and donor engagement workflows through natural conversation.

### What you can do

- **Constituent Oversight** — List and retrieve detailed profiles for donors (individuals and organizations).
- **Transaction Auditing** — Query and inspect donation transactions, pledge payments, and recurring gifts.
- **Fundraising Strategy** — List and monitor campaigns, appeals, and funds to track fundraising progress.
- **Donor Engagement** — Access tasks and notes associated with constituents to maintain strong relationships.
- **CRM Integration** — Retrieve core CRM data including donor IDs and contact history straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Bloomerang API Key
3. Start managing your donor relationships from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Development Directors** — quickly check fundraising totals and campaign statuses without manual exports.
- **Donor Relations Teams** — retrieve donor histories and notes straight from their workflow tools.
- **Non-Profit Ops** — verify transaction details and fund allocations using natural language.


## Available Tools (10)
- **create_constituent**: Create a new individual constituent
- **list_campaigns**: List all fundraising campaigns
- **list_constituents**: List all constituents (donors)
- **list_tasks**: List constituent tasks
- **list_transactions**: List all transactions
- **get_constituent**: Get details of a specific constituent
- **get_transaction**: Get specific transaction details
- **list_appeals**: List all fundraising appeals
- **list_funds**: List all fundraising funds
- **list_notes**: List constituent notes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bloomerang** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our donors in Bloomerang."

**🤖 AI Agent:**
> I've retrieved your constituents. You have 3 recent profiles: 'Alice Johnson' (ID: con_1), 'Global Foundation' (ID: con_2), and 'Mark Smith' (ID: con_3).

---

**👤 You:**
> "Show the fundraising campaigns we have running."

**🤖 AI Agent:**
> Retrieving campaigns... You have 2 active campaigns: 'Annual Fund 2024' (ID: camp_1) and 'Capital Building Project' (ID: camp_2).

---

**👤 You:**
> "Find the last 5 transactions recorded."

**🤖 AI Agent:**
> I've found the 5 most recent transactions. Notable entries include a $500 donation from Alice Johnson and a $1,000 pledge payment from the Global Foundation.


## ❓ FAQ

**Q: Can I check the total donation history for a specific donor?**
Yes! Use the `get_constituent` tool with the Constituent ID to see their core profile, and use `list_transactions` to audit their individual gifts and pledges recorded in Bloomerang.

**Q: How do I list all active fundraising campaigns?**
Simply ask the agent to `list_campaigns`. It will retrieve all fundraising campaigns configured in your Bloomerang CRM for your review.

**Q: Does the integration allow creating new donation transactions?**
Currently, the toolset focuses on querying and auditing (listing constituents, checking transactions). For processing active payments and creating complex financial records, we recommend using the Bloomerang web interface or official forms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bloomerang](https://vinkius.com/mcp/bloomerang)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bloomerang** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bloomerang` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bloomerang** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bloomerang": {
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
