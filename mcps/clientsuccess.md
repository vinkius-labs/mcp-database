# ClientSuccess MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clientsuccess)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage customer success and retention via ClientSuccess — track client health, monitor subscriptions, and manage success cycles directly from any AI agent.

## Description
Connect your **ClientSuccess** account to any AI agent and take full control of your customer success operations through natural conversation. Streamline how you manage account health and revenue retention natively.

### What you can do

- **Client Oversight** — List and retrieve details for all clients, including health scores and status natively
- **Subscription Intelligence** — Access and monitor all subscriptions and contracts associated with specific clients flawlessly
- **Success Cycle Tracking** — Monitor onboarding and success cycles to ensure customer goals are met securely
- **Interaction Auditing** — List and review internal notes and tasks for any specific client flawlessly
- **Contact Logistics** — Access all contacts associated with your clients to maintain relationships securely
- **integrated Visibility** — Retrieve detailed client metadata and profile information directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Enter your ClientSuccess API Key (found in Settings > API)
3. Start managing your customer success from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Success Managers** — monitor account health and review success cycles using natural language
- **Success Operations** — audit subscription data and team tasks without opening the dashboard
- **Sales Teams** — quickly look up client profiles and interaction history straight from their chat interface
- **Leadership** — verify portfolio health and retention metrics across the organization


## Available Tools (8)
- **get_client_success_details**: Get detailed information for a specific client
- **get_my_success_profile**: Retrieve information about the authenticated success manager
- **list_success_clients**: List all clients in ClientSuccess
- **list_client_success_contacts**: List all contacts associated with a specific client
- **list_client_success_notes**: List all internal notes for a specific client
- **list_client_subscriptions**: List all subscriptions and contracts for a specific client
- **list_client_success_cycles**: List all onboarding or success cycles for a client
- **list_client_success_tasks**: List all tasks and to-dos for a specific client


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClientSuccess** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my clients with a 'Risk' health status."

**🤖 AI Agent:**
> Retrieving clients at risk... I found 3 accounts with low health scores: 'Global Tech', 'Startup Inc', and 'Fast Logistics'. Would you like to see their last interaction notes?

---

**👤 You:**
> "Show me the subscriptions for 'Acme Corp'."

**🤖 AI Agent:**
> Checking subscriptions for Acme Corp... They have 1 active contract: 'Enterprise SaaS Plan' ($12,000/year) expiring on Dec 31, 2026. It is set to auto-renew.

---

**👤 You:**
> "What are the pending tasks for the 'Global Tech' account?"

**🤖 AI Agent:**
> Retrieving tasks for Global Tech... There are 3 pending items: 'Quarterly Business Review' (Due tomorrow), 'Update Success Plan', and 'Schedule Training Session'.


## ❓ FAQ

**Q: Can I see the health score for a specific client?**
Yes! Use the `get_client_success_details` tool with the client ID. The agent will return the success score, health status, and other key metrics for that account.

**Q: How do I check the active onboarding cycles for my accounts?**
Use the `list_client_success_cycles` tool. Your agent will fetch all onboarding and success cycles, allowing you to monitor progress and identify any blocked steps.

**Q: Where do I find my ClientSuccess API Key?**
Log in to your ClientSuccess account and navigate to **Global Settings > API**. You can generate and copy your personal API key from that section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clientsuccess](https://vinkius.com/mcp/clientsuccess)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `clientsuccess` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClientSuccess** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clientsuccess": {
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
