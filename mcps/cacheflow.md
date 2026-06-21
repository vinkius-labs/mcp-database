# Cacheflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cacheflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Close SaaS deals faster with automated quoting, billing, and subscription management that removes procurement friction.

## Description
Connect your **Cacheflow** account to any AI agent and take full control of your automated sales proposals and checkout workflows through natural conversation.

### What you can do

- **Proposal Orchestration** — List and manage active sales proposals programmatically, including monitoring their status (sent, viewed, signed) and retrieving detailed metadata
- **Approval Workflow Intelligence** — Access your pending approval requests to maintain a high-velocity sales cycle and oversee the internal signing pipeline in real-time
- **CRM Ecosystem Sync** — Programmatically trigger the synchronization of proposal data to your connected Salesforce or HubSpot instance to ensure high-fidelity records
- **Customer Oversight** — Retrieve complete directories of external customers synced from your CRM to maintain a perfectly coordinated relationship ecosystem
- **Revenue Visibility** — Access specific proposal details and monitor sales performance metrics directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Cacheflow dashboard (Settings > API)
3. Identify your **Subdomain** (e.g., 'acme' from acme.getcacheflow.com)
4. Start managing your proposal-to-cash flow from Claude, Cursor, or any MCP client

No more manual status checking of individual proposals or missing high-intent buyer views. Your AI acts as your dedicated sales operations and revenue coordinator.

### Who is this for?

- **Sales Operations Leads** — instantly retrieve proposal summaries and check approval statuses using natural language commands
- **Account Executives (AEs)** — automate the creation of professional quotes and trigger CRM syncing without leaving your workspace
- **Finance Teams** — monitor the transition from proposal to active checkout through simple AI queries


## Available Tools
- **create_proposal**: Pass data as a JSON string.

Create a new sales proposal
- **get_approval_requests**: List pending approvals for me
- **get_proposal_details**: Get specific proposal details
- **list_customers**: List external customers
- **list_proposals**: List all sales proposals
- **sync_to_crm**: Sync proposal to CRM


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cacheflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active sales proposals in my account."

**🤖 AI Agent:**
> I've retrieved your active proposals. You have 3 documents awaiting signature, including 'Enterprise License - Acme Corp' (ID: prop_123). Would you like to check if they've viewed the document yet?

---

**👤 You:**
> "Show my pending internal approval requests."

**🤖 AI Agent:**
> Accessing approval queue... You have 2 pending requests: one for 'Q2 Product Bundle' requiring VP signature and another for 'Partner Discount' (ID: app_456). Shall I provide the high-fidelity metadata for these?

---

**👤 You:**
> "Sync proposal 'prop_123' to HubSpot."

**🤖 AI Agent:**
> CRM sync triggered! I've initiated the data push for proposal prop_123 to your connected HubSpot instance. Your deal records will be updated automatically. Need help with any other CRM task?


## ❓ FAQ

**Q: How do I find my Cacheflow API Key?**
Log in to your dashboard, navigate to **Settings** > **API**, and generate or copy your secret access token.

**Q: What is my subdomain in Cacheflow?**
Your subdomain is the first part of your Cacheflow URL. For example, if you access at `acme.getcacheflow.com`, your subdomain is `acme`.

**Q: Can I trigger a CRM sync via AI?**
Yes! Use the `sync_to_crm` tool and provide a specific proposal ID to immediately push data to your connected Salesforce or HubSpot instance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cacheflow](https://vinkius.com/mcp/cacheflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cacheflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cacheflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cacheflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cacheflow": {
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
