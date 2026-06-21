# Mockaroo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mockaroo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate realistic dummy data — audit schemas and field types via AI.

## Description
Empower your AI agent to orchestrate your entire data synthesis workflow with **Mockaroo**, the professional engine for realistic dummy data. By connecting Mockaroo to your agent, you transform complex data generation into a natural conversation. Your agent can instantly generate thousands of rows of data, audit saved schemas, and retrieve available field types without you ever touching a technical configuration page. Whether you are testing application performance or building realistic prototypes, your agent acts as a real-time data architect, ensuring your test environments are always powered by high-quality, diverse data.

### What you can do

- **Data Synthesis** — Generate hundreds of realistic records based on custom field definitions and retrieve them in JSON format instantly.
- **Schema Oversight** — Browse your saved Mockaroo schemas to maintain a clear view of your configured data structures.
- **Field Intelligence** — List all available field types in the Mockaroo catalog to identify the perfect markers for your test data.
- **Template Discovery** — Generate data using specific saved schemas to ensure consistency across different test cycles.
- **Dataset Management** — List your uploaded datasets to maintain strict organizational control over your reference data.

### How it works

1. Subscribe to this server
2. Enter your Mockaroo API Key
3. Start managing your data synthesis through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — monitor test data quality and retrieve realistic records straight from your workflow.
- **Backend Developers** — verify data structures and audit schema definitions for API testing.
- **Product Managers** — perform rapid audits of prototype data and identify missing field types through natural language.
- **Operations Leads** — automate data synthesis querying to orchestrate cross-functional development teams smoothly.


## Available Tools
- **generate_mock_data**: Generate dummy data based on a list of fields
- **generate_from_schema**: Generate data using a saved schema name
- **list_datasets**: List uploaded datasets in Mockaroo
- **list_schemas**: List saved schemas in your Mockaroo account
- **list_field_types**: List all available field types for generation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mockaroo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate 10 rows of mock data with 'id' (Row Number) and 'name' (Full Name) using Mockaroo."

**🤖 AI Agent:**
> I've generated 10 records for you! The data includes unique IDs and realistic names like 'John Doe' and 'Jane Smith'. Would you like the JSON output or more rows?

---

**👤 You:**
> "List all my saved schemas in Mockaroo."

**🤖 AI Agent:**
> I've retrieved your schemas. You have 5 saved structures, including 'User Profile' and 'Sales Report'. Which one would you like to use for data generation?

---

**👤 You:**
> "Generate 50 rows using my schema named 'TestUsers'."

**🤖 AI Agent:**
> Data generation complete! I've retrieved 50 rows following the 'TestUsers' structure. I can provide a summary of the generated records if you'd like.


## ❓ FAQ

**Q: How do I find my Mockaroo API Key?**
Log in to your [**Mockaroo account**](https://mockaroo.com/api_keys), and you will find your API Key on the API Keys page. Copy and paste it below.

**Q: Can the agent use my saved schemas?**
Yes. Use the `generate_from_schema` tool providing the name of your saved schema. Your agent will generate data following that specific structure instantly.

**Q: Is it possible to list all available field types?**
Yes. The `list_field_types` tool returns the full catalog of Mockaroo field types, allowing you to audit available markers for your data generation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mockaroo](https://vinkius.com/mcp/mockaroo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mockaroo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mockaroo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mockaroo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mockaroo": {
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
