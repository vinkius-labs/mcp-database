# Honeycomb MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/honeycomb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Automate observability via Honeycomb — manage datasets, queries, and markers directly from any AI agent.

## Description
Connect your **Honeycomb.io** observability platform to any AI agent and take full control of your telemetry data, query specifications, and incident markers through natural conversation.

### What you can do

- **Dataset Oversight** — List all event sources, retrieve detailed metadata, and monitor last access times for your datasets.
- **Query Management** — Define new query specifications and execute them to retrieve granular performance insights.
- **Marker Automation** — Create timeline annotations (e.g., for deployments or outages) to contextualize your data visualization.
- **Schema Insights** — List and inspect columns within specific datasets to understand your event structure.
- **Team Collaboration** — Access shared boards and retrieve information about your Honeycomb team configuration.
- **Incident Analysis** — Use AI to run complex queries and retrieve results for rapid troubleshooting and RCA.

### How it works

1. Subscribe to this server
2. Enter your Honeycomb API Key and select your Region (US or EU)
3. Start querying your telemetry from Claude, Cursor, or any MCP-compatible client

No more manual configuration of complex query DSLs for simple status checks. Your AI assistant acts as a dedicated Observability Engineer or SRE Analyst.

### Who is this for?

- **SREs & DevOps** — instantly retrieve query results and create markers during incident response.
- **Software Engineers** — monitor the performance of new deployments by inspecting specific dataset trends.
- **Platform Leads** — maintain a real-time overview of dataset usage and board sharing across the organization.


## Available Tools
- **create_marker**: Pass details as a JSON string in "body_json" (requires message). Use "__all__" for team-wide markers.

Create a new marker (e.g., deploy, maintenance) on a dataset timeline
- **create_query_specification**: Pass the specification as a JSON string in "query_json". Returns a query ID for execution.

Create a new query specification for a dataset
- **run_query**: Poll for results using "get_query_result" with the returned result ID.

Execute a query specification and return a result ID
- **get_dataset_details**: Get metadata for a specific dataset
- **get_team_details**: Retrieve information about the Honeycomb team
- **get_query_result**: Retrieve the results of an executed query
- **list_honeycomb_boards**: List all boards (dashboards) shared with the team
- **list_dataset_columns**: List all columns (fields) defined in a specific dataset
- **list_datasets**: Use this to find the "slug" required for markers and queries.

List all datasets in your Honeycomb team
- **list_markers**: List markers (annotations) for a dataset
- **list_queries**: List query specifications for a specific dataset
- **list_triggers**: List triggers (alerts) defined for a dataset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Honeycomb** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all datasets and find one related to 'payment-gateway'."

**🤖 AI Agent:**
> I've retrieved your datasets. I found 'gateway-prod' (Slug: gateway-prod) and 'gateway-staging'. Which dataset's schema would you like to inspect?

---

**👤 You:**
> "Create a marker on all datasets: 'Deploy v2.4.0 started'."

**🤖 AI Agent:**
> Marker created! I've successfully added the annotation 'Deploy v2.4.0 started' to all datasets using the environment-wide slug. You should see this marker appear on your graphs in a few moments.

---

**👤 You:**
> "Execute query ID 'q_99283' for the 'main-api' dataset."

**🤖 AI Agent:**
> Query execution triggered! Your result ID is 'res_552'. I'll wait a few moments for the data to process. Should I retrieve the final results for you now?


## ❓ FAQ

**Q: How do I find my Honeycomb API Key?**
Log in to Honeycomb, go to **Team Settings**, and navigate to the **API Keys** section. You will be able to generate and copy your Team API Key from there. Ensure you also note your account's region.

**Q: Which region should I select?**
If your browser URL starts with `ui.eu1.honeycomb.io`, select **EU**. Otherwise, select **US**. Using the correct region is required for the integration to connect to the right API cluster.

**Q: Can I run a query and get the data back?**
Yes! Use the `run_query` tool with a valid query ID. It will return a result ID, which you can then pass to the `get_query_result` tool once the analysis is complete.

**Q: Is the integration secure for telemetry data?**
Absolutely. The integration uses official Honeycomb Team API keys over HTTPS. Your credentials and queried data are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/honeycomb](https://vinkius.com/mcp/honeycomb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Honeycomb** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `honeycomb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Honeycomb** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "honeycomb": {
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
