# ClientSuccess MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clientsuccess-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Reduce churn and grow accounts with health scoring, engagement tracking, and success playbooks built for customer success teams.

## Description
Connect your **ClientSuccess** customer success platform to any AI agent and simplify how you manage your client relationships, track account health, and monitor service contracts through natural conversation.

### What you can do

- **Client Oversight** — List all managed clients and retrieve detailed metadata, including health scores and success status.
- **Relationship Management** — Manage client contacts, query individual profiles, and create new client records programmatically.
- **Contract Monitoring** — List active and historic service contracts to ensure your renewals and agreements are on track.
- **Segmentation** — Query customer segments to understand your client distribution and categorization.
- **Data Insights** — Fetch complete account metadata and health metrics to identify at-risk customers via AI.
- **Operational Efficiency** — Track your customer success ecosystem directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your ClientSuccess API Key (found in your account settings)
3. Start managing your client relationships from your favorite AI assistant

### Who is this for?

- **Customer Success Managers (CSMs)** — quickly check client health scores and retrieve contact info via simple AI commands.
- **Success Operations** — monitor contract distributions and verify segment metadata directly from the workspace.
- **Product & Leadership Teams** — get instant bird's-eye views of client status and account growth via the AI assistant.


## Available Tools (6)
- **create_client**: Create a new client
- **get_client_details**: Get details for a specific client
- **list_clients**: List ClientSuccess clients
- **list_contacts**: Optionally filter by client ID.

List client contacts
- **list_contracts**: List client contracts
- **list_segments**: List client segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClientSuccess** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active clients in my ClientSuccess account."

**🤖 AI Agent:**
> I've retrieved your client directory. You have 35 active organizations including 'Acme Corp', 'Tech Giant', and 'Global Logistics'. Which one would you like to see the health score for?

---

**👤 You:**
> "Show me the details and health score for client 'Acme Corp' (ID: 10293)."

**🤖 AI Agent:**
> Fetching data... Acme Corp currently has a Health Score of 85/100 (Stable). They have 2 active contracts and their primary contact is Sarah Smith. Shall I retrieve their contract details?

---

**👤 You:**
> "List all my customer segments."

**🤖 AI Agent:**
> Retrieving segments... You have 5 segments configured: 'Enterprise', 'Mid-Market', 'SMB', 'Strategic Accounts', and 'Beta Testers'. Which segment would you like to explore?


## ❓ FAQ

**Q: Can I check a client's health score via AI?**
Yes! Use the `get_client_details` tool and provide the Client ID. Your agent will retrieve the current health score, success status, and metadata.

**Q: How do I list all the contracts associated with my clients?**
Run the `list_contracts` query. The agent will retrieve a history of active and previous service contracts recorded in your ClientSuccess account.

**Q: Is it possible to see the available customer segments via AI?**
Absolutely. Use the `list_segments` query. The agent will retrieve the complete list of customer segments used to categorize your client base.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clientsuccess-alternative](https://vinkius.com/mcp/clientsuccess-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ClientSuccess** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clientsuccess-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClientSuccess** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clientsuccess-alternative": {
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
