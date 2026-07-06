# Better Stack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/better-stack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Monitor uptime and incidents via Better Stack — list monitors, heartbeats, and on-call schedules directly from any AI agent.

## Description
Connect your **Better Stack (formerly Better Uptime)** account to any AI agent and orchestrate your infrastructure monitoring and incident management through natural conversation.

### What you can do

- **Uptime Monitoring** — List, create, and manage all your HTTP, Ping, and Keyword monitors to ensure service availability.
- **Incident Response** — Retrieve real-time updates on active incidents and historical reports for post-mortems.
- **On-Call Coordination** — Access on-call schedules and rotations to see who is responsible for system health.
- **Heartbeat Management** — Monitor cron jobs and recurring tasks through heartbeat monitors.
- **Status Page Oversight** — List and verify your public status pages directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Better Stack API Token
3. Start monitoring your infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — quickly check monitor statuses and incident details during an outage without manual dashboard navigation.
- **Backend Developers** — verify heartbeat logs for cron jobs straight from their code editor.
- **Engineering Managers** — retrieve on-call summaries and incident history for reporting.


## Available Tools (10)
- **list_incidents**: List recent uptime incidents
- **list_monitors**: List all uptime monitors
- **list_on_calls**: List on-call schedules and rotations
- **list_status_pages**: List public status pages
- **update_monitor**: Update an existing monitor
- **create_monitor**: Create a new uptime monitor
- **delete_monitor**: Delete a monitor
- **get_incident**: Get details of a specific incident
- **get_monitor**: Get specific monitor details
- **list_heartbeats**: List all heartbeat monitors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Better Stack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all monitors that are currently down."

**🤖 AI Agent:**
> I've checked your monitors. Currently, 2 services are down: 'Primary API' (ID: mon_123) and 'Auth Gateway' (ID: mon_456). Would you like to see the incident details for these?

---

**👤 You:**
> "Show me the on-call schedule for this week."

**🤖 AI Agent:**
> Retrieving on-call data... For the 'Core Infrastructure' rotation, Sarah Miller is on-call until Friday, and John Doe will take over for the weekend.

---

**👤 You:**
> "Check status of heartbeat 'daily-backup'."

**🤖 AI Agent:**
> The heartbeat 'daily-backup' (ID: hb_992) is currently healthy. Its last ping was received 2 hours ago, which is within the expected 24-hour window.


## ❓ FAQ

**Q: Can I check if a specific website is down using the agent?**
Yes! Use the `list_monitors` tool to see the status of all your monitored URLs. You can also use `get_monitor` with a specific ID to see its current status and last checked timestamp.

**Q: How do I see who is currently on-call?**
Simply ask the agent to `list_on_calls`. It will retrieve the current schedules and rotations, showing you who is responsible for incident response right now.

**Q: Does the integration allow me to create a new heartbeat monitor?**
Currently, the toolset focuses on managing monitors and retrieving incident/on-call data. You can list and inspect heartbeats, but for creating new monitors with complex notification rules, we recommend using the Better Stack dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/better-stack](https://vinkius.com/mcp/better-stack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Better Stack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `better-stack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Better Stack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "better-stack": {
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
