# Celigo integrator.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/celigo-integratorio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage integrations and automation flows via Celigo — trigger flows, monitor errors, and audit connections directly from any AI agent.

## Description
Connect your **Celigo integrator.io** account to any AI agent and take full control of your iPaaS (Integration Platform as a Service) operations through natural conversation. Streamline business process automation and data synchronization.

### What you can do

- **Integration Oversight** — List and retrieve details for all active integrations and configured flows natively
- **Flow Control** — Trigger specific integration flows to run on-demand and monitor their status flawlessly
- **Connectivity Audit** — List all active connections and verify their current operational state securely
- **Error Monitoring** — Retrieve recent integration errors to identify and resolve synchronization issues in real-time
- **Data Logistics** — List and manage exports and imports across your various connected applications flawlessly
- **Operational Visibility** — Get detailed flow information and execution logs directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Celigo API Token (obtained from Resources -> API Tokens)
3. Start managing your automations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **IT Administrators** — monitor integration health and trigger manual flow runs using natural language
- **Integration Specialists** — audit connections and review error logs without opening the complex iPaaS dashboard
- **Business Analysts** — verify data synchronization status between ERP, CRM, and E-commerce systems straight from their chat interface
- **Operations Teams** — quickly check the status of specific data imports or exports


## Available Tools (8)
- **list_integration_flows**: List all integration flows
- **get_flow_details**: Get details for a specific flow
- **list_integration_connections**: List all active connections
- **list_integration_errors**: List recent integration errors
- **list_integration_exports**: List configured exports
- **list_integration_imports**: List configured imports
- **list_integrations**: io.

List all integrations
- **run_integration_flow**: Trigger a specific integration flow to run


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Celigo integrator.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my integrations in Celigo."

**🤖 AI Agent:**
> Retrieving your integrations... I found 4: 'NetSuite to Shopify', 'Salesforce to Zendesk', 'Slack Notifications', and 'Inventory Master'. Would you like to see the flows for any of these?

---

**👤 You:**
> "Run the flow with ID 654321."

**🤖 AI Agent:**
> Triggering flow 654321 ('Shopify Orders Sync')... The run has been started successfully in integrator.io. I'll monitor for any immediate errors.

---

**👤 You:**
> "Check for recent integration errors."

**🤖 AI Agent:**
> Scanning for errors... I found 2 recent errors in the 'Salesforce to Zendesk' integration related to mapping. Would you like the full error details?


## ❓ FAQ

**Q: Can I manually start an integration flow?**
Yes! Use the `run_integration_flow` tool with the flow's unique ID. The agent will trigger the execution in Celigo immediately.

**Q: How do I see if any integrations have errors?**
Use the `list_integration_errors` tool. Your agent will fetch the most recent synchronization errors, helping you identify and troubleshoot issues.

**Q: Where do I generate my Celigo API Token?**
Log in to integrator.io, go to 'Resources' in the top menu, then select 'API Tokens'. You can create a new token there (requires Admin permissions).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/celigo-integratorio](https://vinkius.com/mcp/celigo-integratorio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Celigo integrator.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `celigo-integratorio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Celigo integrator.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "celigo-integratorio": {
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
