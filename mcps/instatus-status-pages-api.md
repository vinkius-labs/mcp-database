# Instatus (Status Pages API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/instatus-status-pages-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate your status pages via Instatus — manage incidents, update component statuses, and monitor system health directly from any AI agent.

## Description
Connect your **Instatus** account to any AI agent to streamline your incident communication and status monitoring through natural conversation.

### What you can do

- **Page Management** — List all your status pages and retrieve specific page details and configurations
- **Incident Reporting** — Create, update, and resolve incidents (`add_incident`) to keep your users informed in real-time during outages
- **Component Control** — Update the status of specific infrastructure components (`update_component`) like APIs, Databases, or Websites
- **System Health** — List all active incidents and maintenance windows to get a bird's-eye view of your service availability

### How it works

1. Subscribe to this server
2. Enter your Instatus API Key
3. Start managing your status pages from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SRE Teams** — instantly update status pages during critical outages without leaving your terminal or IDE
- **Customer Support** — check current system health and incident history to provide accurate updates to users without checking multiple dashboards
- **Product Managers** — monitor service uptime and review incident response history directly through AI-generated reports


## Available Tools (28)
- **add_metric**: Add a new metric
- **add_subscriber**: Add a new subscriber
- **add_subscribers_bulk**: Add multiple subscribers (max 100)
- **add_teammate**: Add a team member
- **create_component**: Create a new component
- **create_incident_from_template**: Create an incident using a template
- **create_incident**: Create a new incident
- **create_maintenance**: Create a new maintenance
- **delete_component**: Delete a component
- **delete_incident**: Delete an incident
- **delete_maintenance**: Delete a maintenance
- **delete_metric_datapoints**: Delete datapoints from a metric
- **get_component**: Get a specific component
- **get_incident**: Get a specific incident
- **get_maintenance**: Get a specific maintenance
- **list_components**: Get all components for a page
- **list_incidents**: Get all incidents for a page
- **list_maintenances**: Get all maintenances for a page
- **list_metrics**: Get all metrics for a page
- **list_subscribers**: Get all subscribers for a page
- **list_teammates**: Get all teammates for a page
- **remove_subscriber**: Remove a subscriber
- **remove_teammate**: Remove a team member
- **update_component**: Update an existing component
- **update_incident**: Update an existing incident
- **update_maintenance**: Update an existing maintenance
- **add_metric_datapoint**: Add a datapoint to a metric
- **add_metric_datapoints_bulk**: Add multiple datapoints to a metric


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Instatus (Status Pages API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Instatus status pages."

**🤖 AI Agent:**
> I've retrieved your pages. You have one active page: 'Cloud Services Status' (ID: cl-12345). Would you like to check its components or incidents?

---

**👤 You:**
> "Report a 'Major Outage' incident for the API on page cl-12345."

**🤖 AI Agent:**
> I've created the incident 'Major Outage' for page cl-12345. The status is now live on your page and users have been notified.

---

**👤 You:**
> "Update the 'Database' component status to 'OPERATIONAL' on page cl-12345."

**🤖 AI Agent:**
> The 'Database' component on page cl-12345 has been successfully updated to 'OPERATIONAL'.


## ❓ FAQ

**Q: Can I update the status of a specific component like 'API' or 'Database'?**
Yes! Use the `update_component` tool by providing the Page ID and Component ID. You can set the status to 'OPERATIONAL', 'PARTIAL_OUTAGE', 'MAJOR_OUTAGE', or 'UNDER_MAINTENANCE' instantly.

**Q: How do I list all current incidents for a specific status page?**
Simply ask the agent to run the `list_incidents` action for your target Page ID. It will return a list of all recorded incidents, including their current status and history.

**Q: Is it possible to create a new incident report through the AI?**
Absolutely. Use the `add_incident` tool. You can provide a name, message, and status, and the AI will publish the incident to your Instatus page immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/instatus-status-pages-api](https://vinkius.com/mcp/instatus-status-pages-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Instatus (Status Pages API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `instatus-status-pages-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Instatus (Status Pages API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "instatus-status-pages-api": {
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
