# ArborNote MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arbornote)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage arboricultural surveys, tree inventories, and environmental assessments with specialized forestry field tools.

## Description
Connect your **ArborNote** account to any AI agent and take full control of your tree care and landscaping business operations through natural conversation.

### What you can do

- **Client Relationship Orchestration** — List and manage your entire client directory programmatically, including creating new records and retrieving high-fidelity profile metadata
- **Proposal & Estimate Intelligence** — Monitor the status of active proposals and retrieve detailed high-fidelity cost estimates to coordinate your sales pipeline in real-time
- **Work Order & Project Management** — Programmatically track approved work orders and project milestones to oversee your field operations and team distribution efficiently
- **Financial Visibility Monitoring** — Access invoice histories and retrieve high-fidelity financial metrics to maintain perfectly coordinated revenue operations
- **Operational Monitoring** — Access organization-level metadata and verify active webhooks directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your ArborNote dashboard (Settings > API)
3. Start managing your green assets and client pipeline from Claude, Cursor, or any MCP client

No more manual logging into individual project portals or missing critical proposal views. Your AI acts as your dedicated operations coordinator and business analyst.

### Who is this for?

- **Arborists & Field Managers** — instantly retrieve work order details and update project statuses using natural language commands
- **Sales & Office Staff** — automate the creation of client profiles and monitor proposal health without leaving your workspace
- **Business Owners** — monitor financial performance and organizational metadata through simple AI queries


## Available Tools (12)
- **get_arbornote_project**: Get specific project
- **get_arbornote_proposal**: Get specific proposal
- **list_arbornote_clients**: List all clients
- **list_arbornote_projects**: List active projects
- **list_arbornote_proposals**: List proposals
- **list_arbornote_schedules**: List schedules
- **list_arbornote_webhooks**: List active webhooks
- **update_arbornote_client**: Update an existing client
- **check_api_health**: Verify ArborNote API connectivity
- **create_arbornote_client**: Create a new client
- **get_arbornote_client**: Get specific client
- **get_arbornote_metrics**: Get financial metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ArborNote** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active proposals in my ArborNote account."

**🤖 AI Agent:**
> I've retrieved your active proposals. You currently have 5 estimates awaiting approval, including 'Oak Pruning at 123 Maple St'. Would you like the detailed high-fidelity cost breakdown for any of these?

---

**👤 You:**
> "Show the status of my current work orders."

**🤖 AI Agent:**
> Accessing work orders... You have 3 approved jobs currently in progress and 2 scheduled for tomorrow. All field crews are within high-fidelity operational norms. Shall I retrieve the specific tasks for the 'Riverfront Project'?

---

**👤 You:**
> "Create a new client 'John Doe' (john@example.com) and update his phone to '+15550123'."

**🤖 AI Agent:**
> Client orchestrated! I've successfully created the profile for John Doe (ID: cli_456) and applied the high-fidelity phone update. He is now active in your CRM and ready for a new proposal. Shall I list your available service types?


## ❓ FAQ

**Q: How do I find my ArborNote API Key?**
Log in to your account, navigate to **Settings** > **API**, and generate or copy your unique secret access key.

**Q: Can I update client details via AI?**
Yes! The `update_arbornote_client` tool allows your agent to modify names, emails, and phone numbers for existing records programmatically.

**Q: How do I check financial metrics?**
Use the `get_arbornote_metrics` tool to retrieve a high-fidelity summary of your agency's financial and operational performance data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arbornote](https://vinkius.com/mcp/arbornote)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ArborNote** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `arbornote` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ArborNote** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arbornote": {
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
