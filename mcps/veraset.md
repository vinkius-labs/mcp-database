# Veraset MCP Server

Equip your agent to seamlessly query Veraset's mobility datasets. Run geospatial SQL, extract insights, and manage S3 buckets.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/veraset)

## Overview
**Category:** data-analytics
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Veraset** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/veraset](https://vinkius.com/mcp/veraset)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
