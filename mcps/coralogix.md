# Coralogix MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coralogix)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops-cicd](../categories/devops-cicd.md)

Manage observability, logs, and parsing rules via Coralogix — ingest logs, monitor SLOs, and control Grafana dashboards directly.

## Description
Connect your **Coralogix** account to any AI agent to take full control of your observability and log management workflows through natural conversation.

### What you can do

- **Log Ingestion** — Send logs directly to Coralogix with specific severity levels and metadata using `send_logs`.
- **Parsing Rules** — Retrieve, create, or delete log parsing rule groups to restructure your data flow efficiently.
- **SLO Management** — Programmatically create, list, and delete Service Level Objectives (SLOs) to maintain system reliability.
- **TCO Optimization** — Manage Total Cost of Ownership (TCO) policy overrides to optimize log storage and costs.
- **Grafana Integration** — Search and create Grafana dashboards or retrieve the home dashboard configuration.
- **Deployment Tracking** — Mark releases or deployments using version tags to correlate changes with system behavior.

### How it works

1. Subscribe to this server
2. Enter your Coralogix API Key and Domain
3. Start managing your observability stack from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate the creation of parsing rules and monitor SLOs without leaving the terminal or chat.
- **SREs** — quickly check TCO overrides and deployment tags during incident response.
- **Developers** — send application logs and verify dashboard configurations directly from the code editor.


## Available Tools (17)
- **get_rules**: Get all parsing rules
- **get_tco_overrides**: Get all TCO policy overrides
- **list_custom_enrichments**: List custom enrichments
- **list_slos**: List all SLOs
- **search_grafana_dashboards**: Search hosted Grafana dashboards
- **create_rule_group**: Create a parsing rule group
- **create_slo**: Create a Service Level Objective (SLO)
- **create_tco_override**: Create a TCO policy override
- **send_logs**: Provide an array of log objects.

Send logs to Coralogix
- **create_version_tag**: Create a version tag
- **delete_custom_enrichment**: Delete a custom enrichment
- **delete_rule_group**: Delete a parsing rule group
- **delete_slo**: Delete an SLO
- **delete_tco_override**: Delete a TCO policy override
- **get_grafana_home**: Get hosted Grafana home dashboard
- **get_rule_group**: Get a specific parsing rule group
- **create_grafana_dashboard**: Create or update a hosted Grafana dashboard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coralogix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all log parsing rules currently active in Coralogix."

**🤖 AI Agent:**
> I've retrieved your parsing rules. You have 3 active rule groups: 'JSON-Parser', 'Nginx-Logs', and 'Security-Events'. Would you like to see the details of a specific group?

---

**👤 You:**
> "Search for Grafana dashboards related to 'Kubernetes'."

**🤖 AI Agent:**
> Searching... I found 2 dashboards: 'K8s Cluster Health' and 'Pod Resource Usage'. Which one would you like to inspect?

---

**👤 You:**
> "Create a version tag named 'v2.4.0' for the 'Payment-Service' application."

**🤖 AI Agent:**
> The version tag 'v2.4.0' has been successfully created for 'Payment-Service'. This deployment is now marked in your Coralogix timeline.


## ❓ FAQ

**Q: Can I programmatically create a version tag for a new deployment?**
Yes! Use the `create_version_tag` tool. You can provide a name for the version and optionally specify the application and subsystem to mark exactly when a release occurred.

**Q: How do I check the current Service Level Objectives (SLOs) configured in my account?**
Simply ask the agent to run the `list_slos` query. It will return all configured SLOs, allowing you to monitor reliability targets directly.

**Q: Is it possible to search for existing Grafana dashboards through the AI?**
Yes. You can use the `search_grafana_dashboards` tool by providing a query string. The agent will return matching dashboards found in your Coralogix-hosted Grafana instance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coralogix](https://vinkius.com/mcp/coralogix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coralogix** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coralogix` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coralogix** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coralogix": {
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
