# Healthchecks.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/healthchecksio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monitor cron jobs and background tasks via Healthchecks.io — list checks, track pings, and manage alerts directly from any AI agent.

## Description
Connect your **Healthchecks.io** account to any AI agent to monitor and manage your cron jobs, background tasks, and scheduled services through natural conversation.

### What you can do

- **Check Management** — List, create, update, and delete monitoring checks for your infrastructure
- **Ping History** — Inspect recent pings and payloads to debug failed tasks or verify successful executions
- **Status Monitoring** — Pause or resume checks and track status 'flips' (up/down transitions) over time
- **Integration Overview** — List configured notification channels to ensure your team is alerted correctly
- **Deep Inspection** — Fetch specific check metadata and ping bodies to understand exactly why a service is failing

### How it works

1. Subscribe to this server
2. Enter your Healthchecks.io API Key
3. Start monitoring your background jobs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly verify the health of scheduled tasks and investigate downtime without leaving the terminal
- **Software Developers** — check if background workers are running correctly during development and debugging
- **SRE Teams** — automate the auditing of monitoring coverage and integration status


## Available Tools (13)
- **create_check**: Use the unique field to upsert if it already exists.

Create a new check
- **get_check**: Get a single check by UUID or unique key
- **get_ping_body**: Get the body of a specific ping
- **get_status**: Check the Healthchecks.io service status
- **list_badges**: io status badges.

List all status badges for the project
- **list_checks**: Can be filtered by tags or slug.

List all checks in the project
- **list_flips**: List status changes (flips) for a check
- **list_pings**: List recent pings for a check
- **pause_check**: Pause a check
- **resume_check**: Resume a check
- **update_check**: Update an existing check
- **delete_check**: Delete a check
- **list_integrations**: List all integrations (channels) in the project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Healthchecks.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active checks and their current status."

**🤖 AI Agent:**
> I've retrieved your checks. You have 3 active monitors: 'Daily Backup' (Up), 'Hourly Sync' (Up), and 'Cleanup Script' (Down). Would you like to see the pings for the 'Cleanup Script'?

---

**👤 You:**
> "Show me the last 5 pings for check uuid '550e8400-e29b-41d4-a716-446655440000'."

**🤖 AI Agent:**
> Here are the last 5 pings for that check. The most recent was 10 minutes ago with a 'success' status. Ping #452 included a payload of 1.2KB. Do you want to inspect the body of any specific ping?

---

**👤 You:**
> "Create a new check named 'Database Backup' with a 24-hour timeout."

**🤖 AI Agent:**
> I've created the 'Database Backup' check. The UUID is 'a1b2c3d4...'. You can now send pings to `https://hc-ping.com/a1b2c3d4...`. I've set the timeout to 86400 seconds as requested.


## ❓ FAQ

**Q: Can I see the specific data sent during a ping to debug a failure?**
Yes. Use the `get_ping_body` tool with the check UUID and ping number to retrieve the exact payload or logs sent by your script during that execution.

**Q: How can I see the history of when my service went down?**
You can use the `list_flips` tool. It provides a history of status changes (from 'up' to 'down' and vice versa) for any specific check within a given timeframe.

**Q: Is it possible to silence a check without deleting it?**
Absolutely. Use the `pause_check` tool to stop monitoring and alerts for a specific check. You can later use `resume_check` to start monitoring again.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/healthchecksio](https://vinkius.com/mcp/healthchecksio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Healthchecks.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `healthchecksio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Healthchecks.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "healthchecksio": {
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
