# Directus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/directus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage any SQL database via Directus — handle collection items, audit schemas and fields, manage users, and track media storage directly from any AI agent.

## Description
Connect your **Directus** instance to any AI agent and take full control of your open-source data platform and headless CMS through natural conversation.

### What you can do

- **Collection Orchestration** — Identify bounded routing spaces inside headless Directus SQL mappers and extract database tables traversing collections natively
- **Item Management** — Provision highly-available JSON payloads to write or update Directus rows, or irreversibly wipe records to clear internal database allocations
- **Schema Auditing** — Enumerate explicitly attached structured rules defining your PostgreSQL tables and execute bulk iterations to track registered system types
- **Metadata Inspection** — Analyze specific localized variables decoding native collection boundaries and extracting hidden tracking configurations seamlessly
- **Field Discovery** — Inspect deep internal arrays defining precisely which fields accept formatting and validate payloads strictly against your DB links
- **Identity Oversight** — Explains explicitly mapped profile arrays iterating the exact users authorized within the DB layer enforcing RBAC boundaries securely
- **Media Storage** — Retrieve the exact structural matching verifying file uploads and generating download routes for active frontends

### How it works

1. Subscribe to this server
2. Enter your Directus Base URL and Static Token (found in User Directory > User > Token)
3. Start managing your data platform from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Database Administrators** — audit schemas and manage users without writing complex SQL or using the Studio interface
- **Full-stack Developers** — create and update records and manage digital assets directly from the IDE or chat
- **Product Teams** — monitor collection data and verify field configurations across different environments
- **Content Editors** — manage headless content and digital assets through natural language conversation


## Available Tools
- **create_cms_record**: Provision a highly-available JSON Payload writing Directus Rows
- **wipe_cms_record**: Irreversibly vaporize explicit App nodes dropping live Rows
- **get_collection_details**: Perform structural extraction of properties driving active Tables
- **list_collection_fields**: Inspect deep internal arrays mitigating specific Column configurations
- **get_single_item**: Retrieve explicit Cloud logging tracing explicit DB Row UUIDs
- **list_schema_collections**: Enumerate explicitly attached structured rules defining PostgreSQL tables
- **list_directus_files**: Retrieve the exact structural matching verifying Media storage
- **list_collection_items**: Identify bounded routing spaces inside Headless Directus SQL mappers
- **list_directus_users**: Identify precise active arrays spanning rented Admin identities
- **patch_cms_record**: Mutate global Web CRM boundaries substituting Database values via ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Directus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all items in the 'articles' collection"

**🤖 AI Agent:**
> Retrieving items from 'articles'... I found 12 records. The top ones include 'Intro to Directus' (ID: 1) and 'Database Design' (ID: 2). I can retrieve the full details for any of these.

---

**👤 You:**
> "Create a new record in 'products': {'name': 'Gaming Mouse', 'price': 50}"

**🤖 AI Agent:**
> Record created! 'Gaming Mouse' has been added to the 'products' collection with ID: 'mouse_123'. The database has been updated with your JSON attributes.

---

**👤 You:**
> "Show me the schema for the 'orders' table"

**🤖 AI Agent:**
> Retrieving fields for 'orders'... This collection includes columns like 'customer_id' (UUID), 'order_date' (Timestamp), 'total_amount' (Decimal), and 'status' (String). I can provide the detailed configuration for each field.


## ❓ FAQ

**Q: Can my agent list all collections and their fields in Directus?**
Yes. Use the 'list_schema_collections' tool to see all tables, and then use 'list_collection_fields' for a specific collection. The agent retrieves the absolute structural details defining precisely which fields accept formatting.

**Q: How do I create a new record in a specific Directus collection?**
Use the 'create_cms_record' tool. Provide the collection name and a JSON payload mapping the columns. Your agent will orchestrate the request to drop the formatted endpoint into your database and return the new UUID.

**Q: Can I audit authorized users and their roles via the agent?**
Absolutely. The 'list_directus_users' tool retrieves the explicitly mapped profile arrays iterating the exact users authorized within the database layer. This helps you monitor RBAC boundaries and organizational identities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/directus](https://vinkius.com/mcp/directus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Directus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `directus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Directus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "directus": {
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
