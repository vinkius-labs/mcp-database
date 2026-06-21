# Veraset MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/veraset)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/veraset-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/veraset-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Equip your agent to seamlessly query Veraset's mobility datasets. Run geospatial SQL, extract insights, and manage S3 buckets.

## Description
Bind the massive scale of **Veraset** geolocation data directly to your preferred AI conversational agent. Eradicate context switching when analyzing billions of Points of Interest (POI) and mobile signal attributes.

### What you can do

- **Live SQL Querying** — Prompt your LLM agent to construct, dispatch, and execute ANSI SQL directly aimed at Veraset databases to compute geolocation aggregates.
- **Rapid Execution Management** — Check on long-running geolocation jobs, pull back the output tables seamlessly, or ruthlessly cancel intensive queries straight from your text box.
- **Dataset Profiling** — Scan all your available Veraset packages, request quick dataset schemas, or instantly preview data samples to ensure accuracy before executing queries.
- **Delivery Bucket Access** — Query the secure S3 delivery prefixes attached to your organization for bulk downloads and dynamically generate pre-signed file keys in seconds.

### How it works

1. Install and subscribe to this connector
2. Authorize it using your private Veraset API Key
3. Start fetching and aggregating geolocation data speaking naturally with Claude, Cursor, or compatible clients.

### Who is this for?

- **Data Scientists & Analysts** — validate the schema and preview raw columns of massive geographic drops directly while coding data-pipelines inside Cursor.
- **Geospatial Engineers** — test SQL queries logically pulling subsets of location signals (Movement/Visits datasets) prior to baking them into Python deployments.
- **Retail Strategy Leads** — ask your assistant to fetch quick summaries of competitive POI foot-traffic anomalies without digging into AWS architectures.


## Available Tools
- **cancel_running_query**: Immediately aborts a currently executing SQL task
- **execute_sql_query**: Provide a dataset ID and ANSI SQL. Returns a query ID.

Starts a new SQL query task against a Veraset dataset
- **generate_download_link**: Generates a temporary pre-signed URL for an S3 file download
- **get_dataset_metadata**: Retrieves technical metadata for a specific mobility dataset
- **get_query_results**: Supports pagination.

Retrieves the result rows from a completed SQL query
- **get_query_status**: Checks the progress of a running SQL query
- **get_dataset_sample**: Retrieves a quick sample of the first few rows of a dataset
- **get_dataset_schema**: Retrieves the column definitions and data types for a dataset
- **list_mobility_datasets**: Identify accessible mobility datasets in Veraset
- **list_s3_delivery_folders**: Lists S3 prefixes where scheduled data drops are delivered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Veraset** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our provisioned delivery folder buckets for S3 mobility packets."

**🤖 AI Agent:**
> I've fetched 3 attached S3 delivery prefixes from your Veraset Organization profile:
- `veraset-delivery-east-1/org/xyz/weekly-visits/`
- `veraset-delivery-east-1/org/xyz/movement-v3/`
- `veraset-delivery-east-1/org/xyz/poi-base/`
Would you like me to instantly generate a secure, temporary download link for a parquet file in the 'weekly-visits' tier?

---

**👤 You:**
> "Get a basic preview 10-row sample from the dataset 'movement_global'."

**🤖 AI Agent:**
> Here is the sample of `movement_global`:

The schema primarily includes `id_type`, `accuracy`, `timestamp`, `latitude`, `longitude`, `country`.

Sample Row 1: `ad_id`, `14.5m`, `2023-11-20T10:11:00Z`, `37.7749`, `-122.4194`, `USA`
Sample Row 2: `ad_id`, `8.0m`, `2023-11-20T10:14:32Z`, `51.5074`, `-0.1278`, `GBR`
...
This validates the coordinate systems are populated.

---

**👤 You:**
> "Execute an aggregation query on 'dataset-v5' grouping total foot traffic by 'store_id' and get the current execution status."

**🤖 AI Agent:**
> I've fired off the custom SQL directly to the cloud execution cluster (Job ID: `veraset-sql-job-4299b`). 

I then instantly checked `getQueryStatus` for you. The infrastructure shows the job status as currently `IN_PROGRESS` at approx `15%`. Total scanned bytes sits around `14.2 GB`.

We can fetch the results dynamically using the `getQueryResultsTool` in a few moments. Hang tight.


## Installation & Usage

To install and use the **Veraset** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/veraset](https://vinkius.com/mcp/veraset)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
