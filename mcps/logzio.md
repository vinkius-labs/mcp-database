# Logz.io MCP Server

Query logs, manage alerts, and monitor triggered events in Logz.io directly from your AI agent using Elasticsearch DSL.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/logzio)

## Overview
**Category:** devops-cicd
**Tools Count:** 31

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


## Available Tools
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


## Installation & Usage

To install and use the **Logz.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/logzio](https://vinkius.com/mcp/logzio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
