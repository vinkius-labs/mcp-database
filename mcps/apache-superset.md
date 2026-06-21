# Apache Superset MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apache-superset)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Connect your AI to Apache Superset. Explore BI dashboards, extract chart data, and run live SQL Lab analytics directly from your terminal.

## Description
Empower your conversational AI with deep Business Intelligence access by integrating the **Apache Superset** MCP connector. Seamlessly navigating complex data ecosystems natively from your LLM text-interface, your agent can comprehensively index your analytical infrastructure—spanning from high-level operational dashboards down to specific raw database connections. Instantly run ad-hoc data investigations utilizing internal SQL Lab queries, retrieve explicit graph metadata, and dynamically aggregate critical business insights without abandoning your development environment.

### What you can do

- **Discover Analytics Surfaces** — Audit your entire BI portal intuitively by executing `list_dashboards` and retrieve exact metric configurations invoking `get_dashboard_details`.
- **Graph & Dataset Inspection** — Inventory active metrics logic seamlessly via `list_charts` (or specify via `get_chart_details`) and map semantic layers dynamically performing `list_datasets`.
- **Uncover Data Architectures** — Examine exact backend storage clusters accurately parsing data availability via `list_databases` natively.
- **Direct SQL Processing** — Interface with your central storage matrices seamlessly by generating raw extractions securely via `execute_sql_query` targeting specific analytic connections.

### How it works

1. Append the Apache Superset MCP module systematically into your operational integrations panel.
2. Configure your agent accurately providing your active `SUPERSET_BASE_URL` alongside your validated `SUPERSET_ACCESS_TOKEN` acquired from Superset's security endpoint.
3. Demand direct analytic insights immediately: "Analyze our main Sales dashboard, retrieve the performance dataset logic, and execute a SQL query filtering for Q3 results directly on its database."

### Who is this for?

- **Data Analysts & Scientists** — Expedite query composition flawlessly extracting dataset contexts and formulating complex SQL checks natively utilizing your AI assistant.
- **Product Management teams** — Check dashboard parameters and inspect metric shifts seamlessly via conversational interfaces over Slack or CLI without learning BI navigation.
- **Data Engineering Leads** — Audit operational reports safely probing exact table usage or testing semantic datasets cleanly isolating anomalies iteratively.


## Available Tools (7)
- **execute_sql_query**: Provide a database ID and the SQL statement.

Executes a SQL query via SQL Lab
- **get_chart_details**: Retrieves details for a specific chart
- **get_dashboard_details**: Retrieves details for a specific dashboard
- **list_charts**: Lists all charts (slices) in Superset
- **list_dashboards**: Lists all available dashboards in Apache Superset
- **list_databases**: Lists connected data source connections
- **list_datasets**: Lists all datasets available for analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apache Superset** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Superset dashboards and tell me which one was updated most recently."

**🤖 AI Agent:**
> Found 5 dashboards. The most recently updated is 'Revenue Overview', last modified 2 hours ago.

---

**👤 You:**
> "Check our database connections to see if our Postgres 'SalesDB' is active."

**🤖 AI Agent:**
> Connecting to backend infrastructures... Yes, 'SalesDB' (ID: 12) is active and running on PostgreSQL. Last connection check returned a 200 OK status.

---

**👤 You:**
> "Run a SQL Lab query to show the top 5 product categories by revenue in SalesDB."

**🤖 AI Agent:**
> Executing pure SQL text against 'SalesDB'... Query processed successfully.
Here are your top 5 categories by revenue:
1. Electronics: $1.2M
2. Apparel: $950K
3. Home Goods: $620K
4. Software: $410K
5. Groceries: $240K


## ❓ FAQ

**Q: Can the AI query databases connected to Superset, such as Presto or Redshift?**
Yes. The `execute_sql_query` tool runs queries through Superset's SQL Lab API, which routes them to whichever database engine you have configured — Presto, Redshift, PostgreSQL, and others.

**Q: Are dashboard access permissions enforced when using the MCP server?**
Yes. All requests are authenticated with your `SUPERSET_ACCESS_TOKEN`, so only the dashboards, charts, and datasets your token has access to will be visible to the AI.

**Q: Can the AI run write queries (INSERT, UPDATE, DELETE) via SQL Lab?**
It depends on your Superset database connection settings. By default, SQL Lab connections are read-only. Write access must be explicitly enabled per database in the Superset admin panel.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apache-superset](https://vinkius.com/mcp/apache-superset)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apache Superset** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `apache-superset` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apache Superset** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apache-superset": {
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
