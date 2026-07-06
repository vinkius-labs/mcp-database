# Stitch Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stitch-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Automate data pipelines via Stitch — manage sources, destinations, and push data directly to your warehouse from any AI agent.

## Description
Connect your **Stitch Data** account to any AI agent to orchestrate your ETL workflows and data ingestion through natural conversation.

### What you can do

- **Source & Destination Management** — List, create, and configure data sources and destinations (Redshift, S3, Snowflake, etc.) directly via the Connect API
- **Data Ingestion** — Push batches of records or raw data to the Import API with schema validation for high-integrity data loading
- **Sync Control** — Manually trigger replication jobs and monitor stream metadata to keep your warehouse up to date
- **Account Administration** — Create client accounts and generate ephemeral sessions for secure frontend integrations
- **Pipeline Monitoring** — Check extraction logs and load statuses to ensure your data pipelines are operating correctly

### How it works

1. Subscribe to this server
2. Enter your Stitch Connect Token, Import Token, and Region
3. Start managing your data infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — quickly check sync statuses and update source configurations without leaving the terminal or IDE
- **Analytics Teams** — push custom data batches to warehouses for ad-hoc reporting or testing
- **Product Managers** — monitor data pipeline health and verify successful loads across multiple client accounts


## Available Tools (21)
- **create_destination**: Configure a destination for an account
- **create_ephemeral_session**: Generate a temporary token for the Connect JavaScript client
- **create_source**: Create a new data source
- **delete_destination**: Remove a destination
- **delete_source**: Delete a source
- **get_import_status**: Does not require authentication.

Check if the Stitch Import API is operating correctly
- **list_destination_types**: g., redshift, s3, snowflake).

List available destination types
- **list_destinations**: List configured destinations
- **list_extractions**: List recent extraction jobs
- **list_loads**: List recent data loading attempts
- **list_source_types**: List available source types
- **list_sources**: List all sources for an account
- **list_streams**: List tables (streams) available in a source
- **push_import_batch**: Recommended for best data typing.

Push a batch of records for a single table to the Import API
- **push_import_data**: Does not enforce schemas.

Push data for one or more tables to the Import API
- **start_sync**: Manually start a replication job
- **update_destination**: Update destination settings
- **update_source**: Update, pause, or unpause a source
- **update_stream_metadata**: Select streams and fields for replication
- **validate_import_data**: Used for testing credentials and request formatting.

Validate data format and credentials without persisting data
- **create_account**: Requires partner credentials.

Create a new Stitch client account (Partners only)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stitch Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my configured data destinations in Stitch."

**🤖 AI Agent:**
> I've retrieved your destinations. You have 2 active destinations: 'Production Redshift' (ID: dest_123) and 'Analytics Snowflake' (ID: dest_456).

---

**👤 You:**
> "Push this batch of user records to the 'users' table using push_import_batch."

**🤖 AI Agent:**
> Processing the batch... The data has been successfully pushed to the 'users' table. Stitch has queued the records for ingestion into your warehouse.

---

**👤 You:**
> "Trigger a manual sync for the source with ID src_987."

**🤖 AI Agent:**
> I've initiated the sync for source src_987. The replication job is now running and you can monitor the progress in the extraction logs.


## ❓ FAQ

**Q: How can I verify if my data format is correct before pushing it to the warehouse?**
You can use the `validate_import_data` tool. It functions exactly like a data push but only tests your credentials and data formatting without actually persisting any records.

**Q: Is there a way to check if the Stitch Import API is currently operational?**
Yes, use the `get_import_status` tool. It checks the operational status of the Import API and returns whether it is functioning correctly.

**Q: How do I see which types of sources I can connect to my Stitch account?**
Run the `list_source_types` tool. It will provide a comprehensive list of all available source connectors supported by Stitch.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stitch-data](https://vinkius.com/mcp/stitch-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stitch Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stitch-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stitch Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stitch-data": {
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
