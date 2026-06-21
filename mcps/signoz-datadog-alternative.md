# SigNoz (Datadog Alternative) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/signoz-datadog-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Monitor infrastructure and manage alert rules via SigNoz — list, create, and update observability alerts directly from your AI agent.

## Description
Connect your **SigNoz** instance to any AI agent to streamline your observability and monitoring workflows. SigNoz provides a powerful open-source alternative to Datadog, and this server allows you to manage your alerting infrastructure through natural conversation.

### What you can do

- **Alert Rule Management** — List all configured alert rules, create new ones, or update existing thresholds and conditions using JSON payloads.
- **Rule Maintenance** — Quickly delete stale or redundant alert rules to keep your monitoring environment clean.
- **Account Validation** — Verify your current service account details and API key permissions instantly to ensure connectivity.
- **Observability Audit** — Fetch all alert configurations to audit your monitoring stack without leaving your code editor.

### How it works

1. Subscribe to this server
2. Enter your SigNoz Instance URL and API Key
3. Start managing your monitoring stack from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate the creation of alert rules during deployment or scaling cycles.
- **SREs** — quickly audit existing alert thresholds and conditions without navigating complex web UIs.
- **Platform Teams** — manage observability configurations across multiple environments via simple chat commands.


## Available Tools (5)
- **create_rule**: g., alert, alert_type, condition, thresholds).

Create a new alert rule
- **delete_rule**: Delete an alert rule
- **get_service_account_me**: Get current service account details
- **list_rules**: Retrieve all configured alert rules
- **update_rule**: Update an existing alert rule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SigNoz (Datadog Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all alert rules in my SigNoz instance."

**🤖 AI Agent:**
> I've retrieved 8 alert rules. Some active rules include 'High CPU Usage' (ID: 1), 'Database Latency' (ID: 2), and 'Service 5xx Errors' (ID: 3). Would you like to see the details for any specific rule?

---

**👤 You:**
> "Show me the details of my current service account."

**🤖 AI Agent:**
> Your API key is valid. You are connected as 'Monitoring-Admin' with the following permissions: [Alerts: Read/Write, Dashboards: Read]. Your account ID is 'sa-99283'.

---

**👤 You:**
> "Delete the alert rule with ID 'alert-123'."

**🤖 AI Agent:**
> The alert rule 'alert-123' has been successfully deleted from your SigNoz instance.


## ❓ FAQ

**Q: Can I list all my current alert rules from SigNoz?**
Yes! Use the `list_rules` tool to fetch all alert rules configured in your SigNoz instance, including their conditions and thresholds.

**Q: How do I verify if my API key is working correctly?**
You can use the `get_service_account_me` tool. It validates your current API key and retrieves the associated service account details.

**Q: Is it possible to create a new alert rule via chat?**
Absolutely. Use the `create_rule` tool by providing the required JSON payload containing the alert type, condition, and thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/signoz-datadog-alternative](https://vinkius.com/mcp/signoz-datadog-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SigNoz (Datadog Alternative)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `signoz-datadog-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SigNoz (Datadog Alternative)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "signoz-datadog-alternative": {
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
