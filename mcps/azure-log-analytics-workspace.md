# Azure Log Analytics Workspace MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/azure-log-analytics-workspace)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/azure-log-analytics-workspace-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/azure-log-analytics-workspace-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it queries logs from a single Azure Log Analytics table. That's its only function, and nothing else. Incredible for giving your AI secure observability.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Azure Log Analytics Workspace** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the last 10 error logs."

**🤖 AI Agent:**
> I queried the logs using `| where SeverityLevel == 'Error' | sort by TimeGenerated desc | limit 10`. Here are the results...

---

**👤 You:**
> "Find logs where the user ID was 'admin' in the last 24 hours."

**🤖 AI Agent:**
> I used `| where TimeGenerated > ago(24h) | where UserId == 'admin'` and found 3 relevant log entries.


## Installation & Usage

To install and use the **Azure Log Analytics Workspace** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/azure-log-analytics-workspace](https://vinkius.com/mcp/azure-log-analytics-workspace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
