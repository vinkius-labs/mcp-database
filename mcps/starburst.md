# Starburst MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/starburst)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/starburst-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/starburst-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect your AI to Starburst Enterprise. Query federated data lakes, manage access roles, and orchestrate complex data environments seamlessly.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Starburst** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active operational catalogs across the current data lake instance, and fetch the underlying schematics of any source containing the designation 'finance' in its structure."

**🤖 AI Agent:**
> Parsing connection parameters effectively iterating across federated network protocols successfully maintaining persistent host authentication securely.

**Catalogs Displayed**: `hive`, `postgres_ops`, `finance_db`.

Extracting schematics specifically querying `finance_db`...
**Schemas detected safely (`list_schemas`)**:
- `public`
- `payroll`
- `audit_logs`

Would you like me to execute a precise subquery mapping tables securely localized within `audit_logs` specifically utilizing advanced conversational routines accurately?

---

**👤 You:**
> "Execute a query to retrieve the top 10 rows from the 'customer_analytics' table located in our 'production_hive' catalog."

**🤖 AI Agent:**
> Executing federated SQL query seamlessly...

**Query Results (`execute_query`)**:
The top 10 rows from `production_hive.customer_analytics` have been successfully retrieved. The dataset includes fields such as `customer_id`, `purchase_history`, and `engagement_score`. Would you like me to aggregate this data safely?

---

**👤 You:**
> "List all registered data products across the Starburst network and check current role assignments to ensure proper access."

**🤖 AI Agent:**
> Analyzing data products and roles securely within the Starburst ecosystem...

**Data Products (`list_data_products`)**:
- `Marketing Insights Dashboard`
- `Global Sales Summaries`

**Role Governance (`list_roles`)**:
Verified active assignments for `analyst_tier_1` and `data_governance_admin`. Access privileges align securely with enterprise standards.


## Installation & Usage

To install and use the **Starburst** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/starburst](https://vinkius.com/mcp/starburst)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
