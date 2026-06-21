# Alation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Data catalog orchestration — search assets, audit metadata, and query data via AI.

## Description
Connect your **Alation** instance to your AI agent to unlock enterprise-grade data intelligence and discovery. From searching for critical data assets across your catalog to auditing table schemas and retrieving saved SQL queries, your agent handles your data governance through natural conversation.

### What you can do

- **Catalog Discovery** — Search for schemas, tables, and data sources using keywords and advanced filters
- **Metadata Auditing** — Retrieve detailed logical and physical metadata, including descriptions, stewards, and tags
- **Lineage Analysis** — Trace data lineage to understand the provenance and impact of your data assets
- **Query Orchestration** — List saved SQL queries and retrieve cached execution results from Alation Compose
- **Custom Field Management** — List and audit custom governance fields associated with your catalog objects

### How it works

1. Subscribe to this server
2. Enter your Alation Instance URL and API Access Token
3. Start discovering and managing your data assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find relevant tables and schemas for reporting and analysis
- **Data Governors** — audit metadata completion and manage custom field values across the catalog
- **Engineers** — trace data lineage and inspect column definitions using simple commands
- **Business Intelligence Leads** — retrieve saved queries and monitor data asset endorsements


## Available Tools
- **search_catalog**: Search for data assets
- **list_data_sources**: List catalog data sources
- **list_schemas**: List schemas in data source
- **list_tables**: List tables in schema
- **list_columns**: List columns in table
- **get_object_metadata**: Get object details
- **list_saved_queries**: List saved SQL queries
- **get_query_results**: Get cached query results
- **list_custom_fields**: List governance fields
- **get_lineage**: Trace data lineage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Alation catalog for tables containing 'Customer ROI'."

**🤖 AI Agent:**
> I've searched your catalog. I found 3 tables related to 'Customer ROI', including 'ROI_Analysis_2025' and 'Customer_Success_Metrics'. Would you like to see the schema details for any of them?

---

**👤 You:**
> "List the last 5 SQL queries I saved in Alation."

**🤖 AI Agent:**
> I've retrieved your recent queries. Your last 5 saved SQL items include 'Monthly Churn Report', 'Revenue by Region', and 'Active User Audit'. Would you like me to fetch the cached results for the Churn Report?

---

**👤 You:**
> "Show the lineage for table 'Orders_Main' in the 'Production' schema."

**🤖 AI Agent:**
> I've retrieved the lineage data for Orders_Main. This table is populated from the 'Raw_Staging' schema and feeds into 2 downstream dashboards: 'Global Sales' and 'Finance Forecast'. Would you like the technical details of the transformation logic?


## ❓ FAQ

**Q: How do I find my Alation API Access Token?**
Log in to Alation, click on your user avatar, and go to **Account Settings** > **Authentication**. You can generate a Refresh Token there, which can then be used to obtain short-lived Access Tokens for the API.

**Q: Can I search for specific table types?**
Yes! The `search_catalog` tool allows you to apply filters by object type (otype), such as `table`, `schema`, or `attribute`. This ensures your search results are highly relevant.

**Q: Does this support viewing data lineage?**
Yes, the `get_lineage` tool retrieves technical metadata describing the relationships and data flow between different assets in your catalog.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alation](https://vinkius.com/mcp/alation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `alation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alation": {
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
