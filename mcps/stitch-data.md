# Stitch Data MCP Server

Automate data pipelines via Stitch — manage sources, destinations, and push data directly to your warehouse from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stitch-data)

## Overview
**Category:** data-analytics
**Tools Count:** 21

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


## Available Tools
- **create_account**: Requires partner credentials.

Create a new Stitch client account (Partners only)
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


## Installation & Usage

To install and use the **Stitch Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stitch-data](https://vinkius.com/mcp/stitch-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
