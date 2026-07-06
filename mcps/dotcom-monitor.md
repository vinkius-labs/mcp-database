# Dotcom-Monitor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dotcom-monitor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Monitor website uptime, page load speed, and server health from multiple global locations with instant alert notifications.

## Description
Connect your **Dotcom-Monitor** monitoring account to any AI agent and simplify how you oversee your website uptime, server performance, and global monitoring locations through natural conversation.

### What you can do

- **Device Oversight** — List all configured monitoring devices (uptime, speed, API) and retrieve detailed configuration metadata.
- **Performance Tracking** — Query historical status data and response times to identify latency trends via AI.
- **Global Monitoring** — List available geographic locations and verify where your checks are running from.
- **Alert Management** — Query configured alert groups and notification teams to ensure your incident response is ready.
- **Platform Analysis** — List available monitoring platforms (ServerView, UserView, WebAPI) to coordinate your checks.
- **Operational Monitoring** — Check real-time device health and verify system connectivity directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Dotcom-Monitor API Key (found in your account settings)
3. Start monitoring your digital assets from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps & SREs** — quickly retrieve historical performance logs and verify device statuses via simple AI commands.
- **IT Managers** — monitor global uptime and verify alert group configurations directly from the workspace.
- **Web Developers** — check response times and verify platform availability via the AI assistant.


## Available Tools (6)
- **list_alert_groups**: List configured alert groups
- **list_monitoring_devices**: List monitoring devices
- **list_monitoring_locations**: List geographic monitoring locations
- **list_available_platforms**: ).

List monitoring platforms
- **get_device_details**: Get details for a specific device
- **get_device_monitoring_history**: Get historical status for a device


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dotcom-Monitor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active monitoring devices in my account."

**🤖 AI Agent:**
> I've retrieved your monitoring devices. You have 5 active monitors including 'Homepage Uptime', 'API Gateway Check', and 'Checkout Flow'. Which one would you like to see detailed status for?

---

**👤 You:**
> "Show me the monitoring history for device 'dev_10293'."

**🤖 AI Agent:**
> Fetching history... For device dev_10293, the uptime over the last 24 hours was 100%. Average response time was 120ms, with a peak of 450ms at 3 AM. Would you like to see the error logs?

---

**👤 You:**
> "What are the available alert groups in my account?"

**🤖 AI Agent:**
> Retrieving alert groups... You have 3 groups configured: 'Core Infrastructure' (Email/SMS), 'Frontend Devs' (Slack), and 'Stakeholders' (Weekly Email Report). Shall I verify the members for any of these?


## ❓ FAQ

**Q: Can I check the uptime status of a specific device via AI?**
Yes! Use the `get_device_details` tool and provide the Device ID. Your agent will retrieve the current operational status and basic performance metrics.

**Q: How do I see the history of response times for a monitor?**
Run the `get_device_monitoring_history` query with your Device ID. The agent will retrieve a historical log of success/failure states and latency data.

**Q: Is it possible to list all geographic monitoring locations via AI?**
Absolutely. Use the `list_monitoring_locations` query. The agent will retrieve the complete list of worldwide regions where Dotcom-Monitor agents are available.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dotcom-monitor](https://vinkius.com/mcp/dotcom-monitor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dotcom-Monitor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dotcom-monitor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dotcom-Monitor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dotcom-monitor": {
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
