# leadtributor.cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leadtributorcloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Distribute leads to your sales team and partner network with routing rules, SLA tracking, and performance analytics.

## Description
Connect your **leadtributor.cloud** account to any AI agent and take full control of your channel lead distribution and automated partner management through natural conversation.

### What you can do

- **Lead Distribution Orchestration** — List and manage all distributed leads programmatically, retrieving detailed partner assignment metadata and acceptance status
- **Partner & Channel Intelligence** — Programmatically retrieve directories of channel partners and access complete high-fidelity performance profiles in real-time
- **Conversion Graph Monitoring** — Access real-time status updates for lead conversion and track individual partner performance directly through your agent
- **Metadata Management** — Programmatically retrieve high-fidelity lead sources and history to maintain a perfectly coordinated audit trail of your channel sales
- **Operational Monitoring** — Verify account-level API connectivity and monitor orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your leadtributor.cloud dashboard (Settings > API)
3. Start orchestrating your channel growth from Claude, Cursor, or any MCP client

No more manual emailing of leads to partners or missing critical conversion updates. Your AI acts as your dedicated channel coordinator and lead architect.

### Who is this for?

- **Channel Managers** — instantly retrieve partner performance recaps and monitor lead distribution using natural language commands
- **Business Development Leads** — verify individual lead metadata and track acceptance rates without leaving your creative workspace
- **Developers** — integrate high-speed leadtributor data into custom partner portals through simple AI queries


## Available Tools (12)
- **add_activity**: Add lead activity
- **check_leadtributor_status**: Verify connectivity
- **create_lead**: Create a lead
- **get_lead**: Get lead details
- **get_partner_stats**: Get partner stats
- **get_partner**: Get partner details
- **list_activities**: List lead activities
- **list_leads_by_partner**: List leads by partner
- **list_leads_by_status**: List leads by status
- **list_leads**: List leads
- **list_partners**: List partners
- **update_lead**: Update a lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **leadtributor.cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all leads distributed to partners this week."

**🤖 AI Agent:**
> I've retrieved your distributed leads. You currently have 10 high-fidelity records sent this week, including 7 accepted and 3 pending. Would you like the detailed partner metadata for the pending items?

---

**👤 You:**
> "Show the conversion status for lead ID 'lead_456'."

**🤖 AI Agent:**
> Distribution intelligence orchestrated! For lead 456, I've verified that it was accepted by 'Partner X' and is currently in the 'Contracting' stage. I've retrieved the high-fidelity activity metadata for your review. Need help notifying the manager?

---

**👤 You:**
> "Check the performance metrics for 'Partner X'."

**🤖 AI Agent:**
> Operational monitoring orchestrated! For Partner X, I've identified a 90% high-fidelity lead acceptance rate and 5 successful conversions this month. Your API connection is healthy. Shall I retrieve the detailed pipeline breakdown for this partner?


## ❓ FAQ

**Q: How do I find my leadtributor.cloud API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique access token from the credentials section.

**Q: Can I check partner acceptance rates via AI?**
Yes! The `list_distributed_leads` tool allows your agent to retrieve high-fidelity status metadata for all leads sent to your channel network.

**Q: How do I list my channel partners?**
Use the `list_leadtributor_partners` tool to retrieve your complete high-fidelity directory along with the unique identifiers for all managed companies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leadtributorcloud](https://vinkius.com/mcp/leadtributorcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **leadtributor.cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `leadtributorcloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **leadtributor.cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leadtributorcloud": {
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
