# Upper Route Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/upper-route-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan delivery routes for multiple drivers with optimization algorithms that minimize drive time and maximize daily stops.

## Description
Connect your **Upper Route Planner** account to any AI agent and take full control of your delivery logistics and high-fidelity route orchestration through natural conversation.

### What you can do

- **Route Portfolio Orchestration** — List all optimized delivery routes, retrieve detailed high-fidelity status metadata, and monitor route duration programmatically
- **Stop & Task Intelligence** — Access your complete directory of high-fidelity route stops and tasks to stay on top of field delivery progress in real-time
- **Logistics Provisioning** — Programmatically generate new high-fidelity delivery tasks with precise time windows and customer metadata directly through your agent
- **Driver Monitoring Architecture** — Access high-fidelity driver assignments and resource allocation details to understand and orchestrate your field workforce
- **Stop Detail Discovery** — Access complete high-fidelity metadata for specific delivery stops to maintain perfect contextual alignment for every parcel
- **Operational Monitoring** — Verify account-level API connectivity and monitor route orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your Upper dashboard (Settings > Web Service API)
3. Start managing your delivery growth from Claude, Cursor, or any MCP client

No more manual route checking or missing stop updates. Your AI acts as your dedicated logistics coordinator and route architect.

### Who is this for?

- **Logistics Managers** — instantly retrieve route statuses and monitor driver progress using natural language commands without leaving your creative workspace
- **Operations Leads** — verify high-fidelity delivery metadata and manage task priority to ensure healthy field operations
- **Dispatchers** — analyze technical route efficiency and monitor task volume through simple AI queries


## Available Tools
- **create_upper_delivery_task**: Add a delivery task
- **list_upper_drivers**: List delivery drivers
- **get_upper_route_stop**: Get specific route stop
- **list_upper_routes**: List delivery routes
- **get_upper_stop_details**: Get stop details
- **check_upper_status**: Check API Status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Upper Route Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all delivery routes scheduled for today."

**🤖 AI Agent:**
> I've retrieved your routes. You currently have 8 active high-fidelity routes, including 'North Sector Loop' (Driver: Alex) and 'Downtown Express'. Would you like to see the detailed stop metadata for any of them?

---

**👤 You:**
> "Create a new delivery task for '123 Tech St' with contact 'John Doe'."

**🤖 AI Agent:**
> Logistics provisioned! I've successfully generated a new high-fidelity delivery task for 'John Doe' at '123 Tech St'. This record is now live in Upper. Shall I verify the available route technical windows for assignment?

---

**👤 You:**
> "Check the status of route stop 'stop_456'."

**🤖 AI Agent:**
> Stop directory orchestrated! Stop 'stop_456' is currently 'COMPLETED' with a recorded high-fidelity proof of delivery. Your API connection is healthy. Shall I retrieve the detailed timing metadata for this stop?


## ❓ FAQ

**Q: How do I find my Upper API Token?**
Log in to your account, navigate to **Settings** > **Web Service API**, and copy your unique high-fidelity **API Token**.

**Q: Can I check specific stop details via AI?**
Yes! The `get_upper_stop_details` tool allows your agent to retrieve high-fidelity metadata including service time, customer contact, and delivery notes.

**Q: How do I list my optimized routes?**
Use the `list_upper_routes` tool to retrieve the complete high-fidelity directory of routes along with their assigned drivers and status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upper-route-planner](https://vinkius.com/mcp/upper-route-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Upper Route Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `upper-route-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Upper Route Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upper-route-planner": {
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
