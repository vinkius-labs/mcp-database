# Netdata MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/netdata)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Monitor real-time infrastructure metrics, analyze system performance, and track active alerts across your nodes and Netdata Cloud spaces.

## Description
Connect your **Netdata** monitoring infrastructure to any AI agent for instant, real-time observability and performance analysis through natural language.

### What you can do

- **Real-time Metrics** — Fetch granular data from specific charts (CPU, RAM, Disk, Network) using `get_chart_data` to diagnose performance bottlenecks.
- **Agent Health** — Inspect node versions, host information, and enabled features with `get_agent_info` and `list_charts`.
- **Alert Management** — Query active alarms on local agents via `get_alarms` or monitor space-wide critical issues using `list_space_alerts`.
- **Cloud Orchestration** — Navigate your entire infrastructure by listing spaces, rooms, and nodes connected to Netdata Cloud.
- **Scraping & Export** — Retrieve all metrics in a format suitable for external analysis tools using `get_all_metrics`.

### How it works

1. Subscribe to this server
2. Enter your Netdata Cloud Token or Agent URL
3. Start monitoring your infrastructure from Claude, Cursor, or any MCP-compatible client

No more jumping between dashboards to find which node is spiking. Your AI acts as a 24/7 SRE or System Administrator.

### Who is this for?

- **DevOps Engineers** — instantly correlate system alerts with recent deployments without leaving the terminal or IDE.
- **SREs** — automate the retrieval of chart data and alarm statuses to speed up incident response.
- **System Administrators** — manage large-scale node environments by querying spaces and rooms via simple conversation.


## Available Tools
- **get_alarms**: Get current status of all configured alarms
- **get_all_metrics**: Get all metrics for scraping
- **list_charts**: ).

List all available charts on the node
- **get_chart_data**: Fetch metric data from a specific chart
- **get_agent_info**: Get Netdata Agent information
- **list_room_nodes**: List nodes within a specific room
- **list_rooms**: List rooms within a specific space
- **list_space_alerts**: Fetch active alerts across the space
- **list_space_nodes**: List all nodes connected to a space
- **list_spaces**: List all Netdata Cloud spaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Netdata** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current information and version of the Netdata agent."

**🤖 AI Agent:**
> I've retrieved the agent info. The host is 'prod-server-01' running Netdata version v1.44.1 with 128 enabled collectors.

---

**👤 You:**
> "List all available charts on this node so I can see what metrics are being collected."

**🤖 AI Agent:**
> I've compiled the list of charts. You have access to metrics for 'system.cpu', 'system.ram', 'net.eth0', and 45 other dimensions. Which one would you like to analyze?

---

**👤 You:**
> "Are there any active alarms or warnings on the local agent right now?"

**🤖 AI Agent:**
> Checking alarms... I found one warning for 'disk_backlog' on /dev/sda. All other system health checks are currently clear.


## ❓ FAQ

**Q: How can I fetch specific metric data for a chart like CPU usage?**
Use the `get_chart_data` tool. You need to provide the `chart` ID (e.g., 'system.cpu') and optionally specify time ranges like `after` or aggregation methods like `group`.

**Q: Can I see all active alerts across my entire Netdata Cloud space?**
Yes! Use the `list_space_alerts` tool with your `space_id`. It will return all active alerts across all nodes connected to that specific Cloud space.

**Q: How do I list all the nodes available in a specific room?**
Use the `list_room_nodes` tool. You will need to provide both the `space_id` and the `room_id` to filter the nodes within that specific grouping.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netdata](https://vinkius.com/mcp/netdata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Netdata** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `netdata` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Netdata** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "netdata": {
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
