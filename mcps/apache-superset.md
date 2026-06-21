# Apache Superset MCP Server

Connect your AI to Apache Superset. Explore BI dashboards, extract chart data, and run live SQL Lab analytics directly from your terminal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/apache-superset)

## Overview
**Category:** brain-trust
**Tools Count:** 7

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


## Available Tools
- **execute_sql_query**: Provide a database ID and the SQL statement.

Executes a SQL query via SQL Lab
- **get_chart_details**: Retrieves details for a specific chart
- **get_dashboard_details**: Retrieves details for a specific dashboard
- **list_charts**: Lists all charts (slices) in Superset
- **list_dashboards**: Lists all available dashboards in Apache Superset
- **list_databases**: Lists connected data source connections
- **list_datasets**: Lists all datasets available for analysis


## Installation & Usage

To install and use the **Apache Superset** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apache-superset](https://vinkius.com/mcp/apache-superset)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
