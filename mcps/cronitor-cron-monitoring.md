# Cronitor (Cron Monitoring) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cronitor-cron-monitoring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monitor cron jobs, heartbeats, and websites. Track performance, receive alerts, and manage uptime directly from your AI agent.

## Description
Connect **Cronitor** to your AI agent to gain full visibility into your background jobs, heartbeats, and website uptime through natural conversation.

### What you can do

- **Monitor Management** — List, create, and update monitors for cron jobs, heartbeats, and health checks across your entire infrastructure.
- **Real-time Telemetry** — Send pings and job state updates (run, complete, fail) directly to track execution lifecycles.
- **Performance Insights** — Query metrics, aggregates, and site analytics to understand latency, success rates, and system health.
- **Incident Response** — Track active issues, manage status pages, and create maintenance windows to silence alerts during deployments.
- **Infrastructure Control** — Organize monitors into groups, manage notification settings, and audit API keys.

### How it works

1. Subscribe to this server
2. Enter your Cronitor API Key
3. Start monitoring your stack from Claude, Cursor, or any MCP-compatible client

No more jumping between dashboards to check if your nightly backups finished or why a heartbeat is missing. Your AI acts as a 24/7 SRE assistant.

### Who is this for?

- **DevOps Engineers** — instantly check monitor statuses and silence alerts during maintenance without leaving the terminal.
- **Backend Developers** — verify cron job performance and send telemetry pings directly from the code editor.
- **SRE & Ops Leads** — manage status pages and track incident history across multiple environments.


## Available Tools (44)
- **bulk_issues**: Perform bulk actions on issues
- **clone_monitor**: Clone an existing monitor
- **create_api_key**: Create an API key
- **create_status_page_component**: Create a status page component
- **create_environment**: Create an environment
- **create_group**: Create a new monitor group
- **create_issue**: Create a new issue
- **create_maintenance_window**: Schedule a maintenance window
- **create_monitor**: Create a new monitor
- **create_notification**: Create a notification list
- **create_site**: Create a RUM site
- **create_status_page**: Create a status page
- **delete_api_key**: Delete an API key
- **delete_status_page_component**: Delete status page components
- **delete_group**: Delete a monitor group
- **delete_monitor**: Delete a monitor
- **delete_site**: Delete RUM sites
- **delete_status_page**: Delete status pages
- **get_aggregates**: Retrieve rolled-up aggregates
- **get_metrics**: Requires at least one field parameter.

Retrieve performance metrics
- **get_monitor**: Retrieve a specific monitor
- **get_site_errors**: Get site errors
- **list_api_keys**: List API keys
- **list_status_page_components**: List status page components
- **list_environments**: List environments
- **list_groups**: List monitor groups
- **list_issues**: List issues and incidents
- **list_monitors**: List or search monitors
- **list_notifications**: List notification lists
- **list_sites**: List RUM sites
- **list_status_pages**: List status pages
- **pause_group**: Bulk pause or resume a group of monitors
- **pause_monitor**: Use 0 to resume.

Pause or resume a monitor
- **query_site_analytics**: Query site analytics
- **send_telemetry**: link.

Send telemetry events (pings, metrics)
- **update_api_key**: Update an API key
- **update_status_page_component**: Update status page components
- **update_environment**: Update an environment
- **update_group**: Update a monitor group
- **update_issue**: Update an issue state
- **update_monitors**: Create or update monitors in bulk
- **update_notification**: Update a notification list
- **update_site**: Update RUM sites
- **update_status_page**: Update status pages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cronitor (Cron Monitoring)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active monitors and show their current status."

**🤖 AI Agent:**
> I've retrieved your monitors. You have 12 active monitors. 10 are 'Healthy', but 'nightly-db-backup' is currently 'Failing' and 'api-health-check' is 'Paused'.

---

**👤 You:**
> "Get the P50 duration metrics for the last 24 hours."

**🤖 AI Agent:**
> Fetching performance data... The P50 duration across all monitors for the last 24h is 145ms. Would you like to see the breakdown by specific monitor?

---

**👤 You:**
> "Pause the 'data-sync' monitor for the next 4 hours."

**🤖 AI Agent:**
> The 'data-sync' monitor has been successfully paused for 4 hours. Alerts will be silenced until the pause expires or you resume it manually.


## ❓ FAQ

**Q: How can I manually signal that a job has finished successfully?**
You can use the `send_telemetry` tool. Provide the `monitor_key` and set the `state` to 'complete'. This will immediately update Cronitor with the job's success status.

**Q: Is it possible to silence alerts for a specific monitor during maintenance?**
Yes! Use the `pause_monitor` tool with the `monitor_key` and the number of `hours` you want to pause it. Alternatively, use `create_maintenance_window` for broader scheduling.

**Q: How do I check for recent errors on my monitored websites?**
Use the `get_site_errors` tool. It retrieves the most recent error logs and failure details for a specific site monitor, helping you debug downtime quickly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cronitor-cron-monitoring](https://vinkius.com/mcp/cronitor-cron-monitoring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cronitor (Cron Monitoring)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cronitor-cron-monitoring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cronitor (Cron Monitoring)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cronitor-cron-monitoring": {
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
