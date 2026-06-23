# Azure Log Analytics Workspace MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/azure-log-analytics-workspace)
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


## Available Tools (1)
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


## ❓ FAQ

**Q: Why limit the agent to a single Log Table?**
To enforce zero-trust security. A Workspace often contains sensitive audit trails (like AzureActivity or SecurityEvents). By locking the agent to a specific table (e.g., 'AppExceptions'), you prevent it from reading global infrastructure access logs.

**Q: How should I format my KQL queries?**
You do NOT need to include the table name. The MCP engine automatically handles the table prefix. Just pass the KQL operators starting with a pipe. Example: `| where TimeGenerated > ago(1h) | limit 50`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/azure-log-analytics-workspace](https://vinkius.com/mcp/azure-log-analytics-workspace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Azure Log Analytics Workspace** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `azure-log-analytics-workspace` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Azure Log Analytics Workspace** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "azure-log-analytics-workspace": {
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
