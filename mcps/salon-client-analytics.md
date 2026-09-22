# Salon Client Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/salon-client-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Analyze salon engagement, retention, and churn using appointment data.

## Description
This MCP server provides business intelligence for salon owners by analyzing appointment records. It allows AI agents to calculate unique client counts, monitor customer retention rates, identify active clients, and generate churn reports. Use `get_client_statistics` to compare service volume against unique human engagement, or `get_churn_report` to identify lost business by finding clients who have stopped visiting.


## Available Tools (4)
- **get_active_client_count**: Identifies how many clients are currently active
- **get_churn_report**: Identifies lost business by finding clients who have stopped visiting
- **get_client_statistics**: Provides a high-level overview of salon engagement
- **get_retention_metrics**: Answers how well the salon maintains its customer base


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salon Client Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of salon engagement for the first quarter of 2024."

**🤖 AI Agent:**
> In Q1 2024, the salon had 150 unique clients and 450 total appointments, resulting in an average of 3 appointments per client.

---

**👤 You:**
> "How many clients have been active in the last 30 days?"

**🤖 AI Agent:**
> There are 42 active clients who have completed an appointment within the last 30 days.

---

**👤 You:**
> "Who are the clients we have lost? Check for anyone inactive for 60 days as of today."

**🤖 AI Agent:**
> There are 12 churned clients who have not visited in the last 60 days.


## ❓ FAQ

**Q: How does this tool calculate unique clients?**
The unique client count is derived by counting distinct client IDs within the specified date range provided to `get_client_statistics`.

**Q: What defines a churned client?**
A client is considered churned if their most recent appointment was longer ago than the inactivity threshold relative to the analysis date.

**Q: Can I see how many clients returned for a second visit?**
Yes, you can use `get_retention_metrics` to see the number of returning clients and the retention percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/salon-client-analytics](https://vinkius.com/en/ai-agent-connect/salon-client-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salon Client Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salon-client-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salon Client Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salon-client-analytics": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
