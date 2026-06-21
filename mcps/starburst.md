# Starburst MCP Server

Connect your AI to Starburst Enterprise. Query federated data lakes, manage access roles, and orchestrate complex data environments seamlessly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/starburst)

## Overview
**Category:** industry-titans
**Tools Count:** 6

## Description
Integrate the powerful federated data analytics capabilities of **Starburst** directly into your conversational AI workflows. Empower your data engineering and analytics teams to query extensive data lakes, manage organizational roles, and explore detailed schemas without needing to explicitly switch between database clients. Securely map your AI assistant to your Starburst host, enabling natural language orchestration of complex Trino-based data products to accelerate data discovery and governance across your entire enterprise architecture.

### What you can do

- **Federated Query Execution** — Pass complex SQL statements programmatically against your connected data sources utilizing `execute_query`, receiving structured analytic returns directly.
- **Schema & Catalog Discovery** — Actively map your data landscape by inspecting linked databases invoking `list_catalogs`, and drill down into specific table hierarchies using `list_schemas`.
- **Data Product Management** — Manage and retrieve existing analytical data products across the Starburst network systematically validating data definitions using `list_data_products`.
- **Governance & Role Administration** — Inspect access control limitations securely by navigating role assignments formally deploying requests through `list_roles` and evaluating privilege thresholds.

### How it works

1. Install the Starburst MCP connector, binding it inherently to your active LLM assistant.
2. In the MCP configurations, provide your `STARBURST_HOST` and your `STARBURST_TOKEN` to securely establish a persistent communication session.
3. Instruct the AI: "Execute a query listing the top 10 rows from the 'customer_analytics' table located in our 'production_hive' catalog, and summarize the data."

### Who is this for?

- **Data Engineers** — Radically streamline data auditing by parsing schemas, managing catalogs, and iterating over queries utilizing an intuitive conversational interface.
- **Data Analysts** — Explore massive federated datasets without writing rigorous boilerplate connection scripts, leveraging AI to construct and execute complex SQL instantly.
- **Data Governance Managers** — Maintain strict oversight of access limitations continuously verifying role assignments and auditing internal data products natively.


## Available Tools
- **get_query_details**: Retrieves details for a specific SQL query
- **list_catalogs**: g., S3, Snowflake, Iceberg) are connected.

Lists all data catalogs available in Starburst Galaxy
- **list_data_products**: Lists all published data products
- **list_domains**: Lists data product domains
- **list_queries**: Lists recent SQL queries executed in the cluster
- **list_roles**: Lists all security roles in the organization


## Installation & Usage

To install and use the **Starburst** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/starburst](https://vinkius.com/mcp/starburst)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
