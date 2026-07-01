# New Relic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/new-relic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Monitor and query your entire stack via New Relic NerdGraph — track entities, NRQL, and alerts directly from your AI agent.

## Description
Connect your **New Relic** account to your AI agent and gain full visibility into your applications and infrastructure through natural conversation using the powerful NerdGraph GraphQL API.

### What you can do

- **Entity Discovery** — List and search for monitored entities such as APM applications, hosts, containers, and browser apps.
- **Custom Querying** — Execute raw NRQL (New Relic Query Language) strings to retrieve specific datasets and custom metrics.
- **Golden Metrics** — Fetch real-time APM summaries including error rates, Apdex scores, and average response times.
- **Incident Monitoring** — Track active AI-detected issues and open alerts across your accounts.
- **Dashboard Oversight** — List and retrieve configuration details for your custom observability dashboards.
- **Account Management** — Access current user metadata and list all accessible New Relic accounts.
- **SLO Tracking** — Monitor defined Service Level Indicators (SLOs) and performance levels.

### How it works

1. Subscribe to this server
2. Enter your New Relic User API Key
3. Start monitoring your infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **SRE & DevOps Engineers** — quickly check for active incidents or run NRQL queries without opening the browser.
- **Developers** — monitor the health and golden metrics of your applications during deployment or testing.
- **Product Managers** — track SLOs and high-level performance indicators through natural language.


## Available Tools (10)
- **get_apm_summary**: Get APM golden metrics
- **get_dashboard**: Get dashboard configuration
- **list_dashboards**: List New Relic dashboards
- **list_entities**: List monitored entities
- **list_service_levels**: List Service Level Indicators (SLOs)
- **run_nrql**: Execute a NRQL query
- **get_entity_details**: Get specific entity metadata
- **get_me**: Get current user and account info
- **list_accounts**: List accessible New Relic accounts
- **list_alerts**: List active issues and alerts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **New Relic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all APM applications in my account."

**🤖 AI Agent:**
> Retrieving entities... I found 5 APM applications: 'Web-Frontend-Prod', 'Inventory-Service', 'Auth-API', and 2 others. Would you like the golden metrics for 'Web-Frontend-Prod'?

---

**👤 You:**
> "Show me the error rate and response time for application GUID 'MTIzNDU2fEFQTXxBUFBMSUNBVElPTnwxMjM'."

**🤖 AI Agent:**
> Fetching APM summary... For application 'Web-Frontend-Prod', the current error rate is 0.05%, the Apdex score is 0.98, and the average response time is 156ms. These values are within normal operating ranges.

---

**👤 You:**
> "Run NRQL: 'SELECT average(duration) FROM Transaction FACET appName SINCE 1 DAY AGO' for account 12345."

**🤖 AI Agent:**
> Executing NRQL query... The results show the average duration per application over the last 24 hours. 'Web-Frontend' averaged 0.12s, 'Auth-API' averaged 0.08s, and 'DB-Proxy' averaged 0.45s. Shall I format this into a table for you?


## ❓ FAQ

**Q: Where do I find my User API Key?**
In New Relic, go to the account dropdown > API keys. Look for a key of type 'USER'. This is required for NerdGraph access.

**Q: Can I run any NRQL query through this server?**
Yes! Use the `run_nrql` tool and provide your Account ID and the query string. This allows for extremely flexible data retrieval.

**Q: What are APM golden metrics?**
Golden metrics are the most critical performance indicators for an application: Response Time, Throughput, Error Rate, and Apdex (user satisfaction).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/new-relic](https://vinkius.com/mcp/new-relic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **New Relic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `new-relic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **New Relic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "new-relic": {
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
