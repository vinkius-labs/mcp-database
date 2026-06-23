# Logz.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/logzio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops-cicd](../categories/devops-cicd.md)

Query logs, manage alerts, and monitor triggered events in Logz.io directly from your AI agent using Elasticsearch DSL.

## Description
Connect your **Logz.io** observability platform to any AI agent to streamline your DevOps and security workflows. This server allows you to interact with your logs and alerts through natural language.

### What you can do

- **Advanced Log Search** — Execute complex queries using Elasticsearch DSL via the `search_logs` tool and handle large datasets with `scroll_logs`.
- **Alert Management** — List, create, update, and delete alerts. You can also toggle alerts on or off using `enable_alert` and `disable_alert`.
- **Incident Monitoring** — Retrieve a paged list of triggered alert events with `list_triggered_alerts`, filtering by severity or tags to identify critical issues quickly.
- **Security Automation** — Integrate log analysis and alert status checks directly into your incident response or monitoring dashboard.

### How it works

1. Subscribe to this server
2. Provide your Logz.io API Token and specify your region (e.g., US, EU, WA)
3. Start querying your infrastructure logs and managing alerts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly search for error patterns and system logs without switching to the Logz.io UI.
- **SREs** — monitor triggered alerts and adjust alert configurations during on-call rotations.
- **Security Analysts** — audit logs and security rules through a conversational interface to speed up investigations.


## Available Tools (31)
- **create_alert**: Create a new alert
- **create_deployment_markers**: Add deployment markers to annotate Exception graphs in Kibana
- **create_lookup_list**: g., blacklisted IPs) for use in SIEM rules.

Create a lookup list for SIEM rules
- **create_metrics_account**: Create a Metrics account
- **create_security_rule**: Create a new SIEM security rule
- **create_siem_account**: Creates a new SIEM account associated with your main logs account
- **create_snapshot**: Create a Kibana snapshot
- **create_user**: Create a new user
- **delete_alert**: Delete an alert
- **delete_security_rule**: Delete a SIEM security rule
- **delete_user**: Delete a user
- **disable_alert**: Disable an alert
- **enable_alert**: Enable an alert
- **get_lookup_list**: Get a lookup list by ID
- **get_snapshot**: Get a Kibana snapshot
- **list_alerts**: io account.

Returns a list of all configured alerts
- **list_insights**: io.

Retrieves LOGCEPTION and PUBLIC_CI insights detected in your logs
- **list_triggered_alerts**: Returns a paged, filtered list of triggered alert events
- **list_users_recursive**: List all users in main account and sub-accounts
- **list_users**: List users for a single account
- **scroll_logs**: Paginate through large result sets from search
- **search_logs**: Returns up to 10,000 results.

Search account data using Elasticsearch Search API DSL
- **search_lookup_lists**: Search lookup lists
- **search_security_event_logs**: Retrieves the specific logs that caused a security event to trigger
- **search_security_events**: Fetch events triggered by security rules
- **search_security_rules**: Search SIEM security rules
- **suspend_user**: Suspend a user
- **unsuspend_user**: Unsuspend a user
- **update_alert**: Update an existing alert
- **update_security_rule**: Update a SIEM security rule
- **update_user**: Update a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Logz.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for logs with level 'ERROR' in the last 15 minutes using search_logs."

**🤖 AI Agent:**
> I've executed the search. I found 12 error logs. Most of them are related to 'Connection Timeout' in the production cluster. Would you like to see the full details of these entries?

---

**👤 You:**
> "List all configured alerts and tell me which ones are currently disabled."

**🤖 AI Agent:**
> Fetching your alerts... You have 8 alerts configured. Currently, 'High Latency DB' and 'Disk Space Warning' are disabled. The other 6 are active.

---

**👤 You:**
> "Show me the most recent triggered alerts with 'High' severity."

**🤖 AI Agent:**
> I found 3 triggered alerts with High severity: 'API 5xx Spike', 'Unauthorized Access Attempt', and 'Memory Usage Critical'. All were triggered within the last hour.


## ❓ FAQ

**Q: Can I perform complex log searches using Elasticsearch DSL?**
Yes. The `search_logs` tool accepts a full Elasticsearch DSL query object, allowing you to filter, aggregate, and sort your log data with high precision.

**Q: How do I check which alerts have been triggered recently?**
Use the `list_triggered_alerts` tool. You can filter the results by severity, tags, or search for specific alert names to identify active incidents.

**Q: Is it possible to temporarily stop an alert without deleting it?**
Absolutely. You can use the `disable_alert` tool with the specific Alert ID to pause it, and `enable_alert` to turn it back on whenever you're ready.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/logzio](https://vinkius.com/mcp/logzio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Logz.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `logzio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Logz.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "logzio": {
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
