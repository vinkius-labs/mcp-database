# Azure Log Analytics Workspace MCP Server

This MCP does exactly one thing: it queries logs from a single Azure Log Analytics table. That's its only function, and nothing else. Incredible for giving your AI secure observability.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/azure-log-analytics-workspace)

## Overview
**Category:** industry-titans
**Tools Count:** 1

## Description
This server strips away dangerous global Azure permissions. It gives your AI agent one surgical superpower: **the ability to run KQL queries on one specific Log Analytics table.**

By strictly scoping access, your AI can safely troubleshoot application errors, analyze traffic spikes, and monitor infrastructure without ever gaining access to sensitive audit trails globally.

### The Superpowers

- **Absolute Containment:** The agent is strictly locked to query a single table. It cannot search across all workspace logs.
- **Native KQL Power:** Supports full Kusto Query Language syntax, allowing the AI to filter, parse JSON payloads, and extract insights.
- **Plug & Play Troubleshooting:** Instantly gives your agent the eyes and ears it needs to debug production issues autonomously.


## Available Tools
- **query_logs**: Do NOT include the table name in your query operations. The engine automatically prepends the authorized table name. Just provide the KQL operations (e.g., "| where TimeGenerated > ago(1h) | limit 10").

Execute a Kusto (KQL) query against the configured Log Analytics table


## Installation & Usage

To install and use the **Azure Log Analytics Workspace** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/azure-log-analytics-workspace](https://vinkius.com/mcp/azure-log-analytics-workspace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
