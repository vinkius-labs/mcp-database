# CARTO MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/carto)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/carto-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/carto-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Empower your AI agents to execute spatial SQL, generate routes, create driving isolines, and bulk geocode directly on CARTO.

## Description
Connect your **CARTO** platform to any AI agent and take full control of your cloud-native spatial analytics without touching the GIS interface.

### What you can do

- **Spatial SQL & Jobs** — Command explicit SQL queries running directly against your BigQuery, Snowflake, or Redshift warehouse. Execute quick reads or spawn long-running, asynchronous batch transformations.
- **Geocoding & Batching** — Convert unstructured strings into precise lat/lon points. Bulk-process 100s of addresses using CARTO's native Location Data Services (LDS) gracefully.
- **Isolines & Reachability** — Calculate travel-time or distance polygons around origin points to instantly graph accessible zones via cars or walking.
- **Routing** — Generate optimal vector geometry paths connecting two points on the globe, measuring both physical distance and travel time securely.
- **Data Management** — Instruct your agent to list active mapping datasets or import massive external CSV/GeoJSON files directly via public URLs.

### How it works

1. Subscribe to this server
2. Provide your active CARTO Organization and API Key
3. Start mapping, slicing spatial boundaries, and scripting data operations using Claude, Cursor, or any compatible AI

### Who is this for?

- **GIS Analysts & Data Scientists** — Execute testing queries natively and bulk-geocode customer coordinates from a conversational terminal.
- **Retail & Logistics Strategists** — Ask your AI to calculate 15-minute delivery isolines and cross-reference them with population layers using SQL.
- **Data Engineers** — Trigger raw data imports and handle heavy dataset syncs without opening the graphical workspace.


## Available Tools
- **calculate_isoline**: The range parameter is in seconds for time-based isolines. Returns a GeoJSON polygon representing the reachable area. Use for service area analysis, store catchment zones, and logistics planning.

Generate travel-time or travel-distance isoline polygons from a center point using the CARTO LDS Isolines API, producing reachability contours showing areas accessible within a specified time or distance threshold
- **calculate_route**: Returns the route as GeoJSON with total distance (meters) and duration (seconds). Consumes LDS routing credits.

Calculate the optimal driving route between two points using the CARTO LDS Routing API, returning distance, duration, and route geometry suitable for visualization on CARTO maps
- **create_async_sql_job**: "}`. Returns a job_id that can be polled for completion status. Use for ETL operations, materialized view refreshes, and heavy geospatial computations. The job runs in your data warehouse and results are stored there.

Submit a long-running SQL query as an asynchronous batch job via the CARTO SQL Job API, suitable for heavy spatial analytics, large table transformations, and complex multi-join operations that exceed the 60-second synchronous timeout
- **execute_sql_query**: carto.com/api/v2/sql?q=`. The query runs synchronously with a 1-minute timeout. Use for quick analytical queries, spatial joins, and data exploration. For long-running queries exceeding 60 seconds, use the async job endpoint instead. Supports PostGIS/BigQuery spatial functions natively.

Execute an arbitrary SQL query against your CARTO data warehouse connection using the SQL API v2, returning results as JSON rows directly from BigQuery, Snowflake, Redshift, or PostgreSQL
- **geocode_address**: Returns latitude, longitude, and formatted address. Consumes LDS geocoding credits from your CARTO plan. Use sparingly for individual lookups; for bulk operations use the batch endpoint instead.

Forward-geocode a single address string into geographic coordinates using the CARTO Location Data Services (LDS) geocoding endpoint, powered by TomTom or HERE depending on your CARTO plan configuration
- **geocode_batch_addresses**: Designed for bulk processing of customer lists, store locators, and CRM datasets. Consumes LDS credits per address. Returns an array of geocoded results with match quality indicators.

Batch-geocode multiple addresses in a single request using the CARTO LDS batch geocoding API, efficiently converting large address lists into coordinates without making individual API calls per address
- **get_import_status**: Poll periodically until state becomes "complete" or "failure". On success, the response includes the table_name of the newly created dataset in your warehouse.

Check the status of a previously initiated CARTO data import job, returning progress percentage, current state (uploading, importing, complete, failure), and any error details if the import encountered issues
- **import_external_file**: "}`. Supports CSV, GeoJSON, Shapefile (zipped), KML, GPX, and Excel files. Returns an import_id for status tracking. The file is downloaded, parsed, and loaded into your connected data warehouse.

Import an external data file (CSV, GeoJSON, Shapefile, KML) into your CARTO data warehouse by providing a publicly accessible URL, creating a new managed table that can be used for spatial analysis and visualization
- **list_map_datasets**: Returns an array of dataset/visualization objects. Use to discover available data layers, check dataset freshness, and audit organization assets.

List all visualization datasets (maps and tables) available in your CARTO organization, returning metadata including creation dates, privacy settings, table names, and row counts
- **poll_async_job_status**: Poll periodically (every 5-10 seconds) until status changes to "done" or "failed". The response includes created_at, updated_at, and the original query for audit purposes.

Check the execution status of a previously submitted CARTO async SQL job, returning the current state (pending, running, done, failed) and any error messages if the job encountered issues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CARTO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Execute a SQL query limiting to 10 rows on my 'retail_stores' dataset to check the schema."

**🤖 AI Agent:**
> The query executed successfully. The schema for 'retail_stores' includes columns: store_id, revenue, state_code, and geom. Here are the top 3 rows formatted for readability: ...

---

**👤 You:**
> "Take these 5 addresses in Madrid and bulk geocode them to lat/lon coordinates."

**🤖 AI Agent:**
> Batch geocoding completed using CARTO LDS. I have translated the 5 specific text blocks into geo-coded coordinates. Example: Calle de Alcalá, 45, Madrid matches exactly to [40.418, -3.696]. Would you like me to dump this formatted JSON object for you?

---

**👤 You:**
> "Generate a 15-minute drive-time isoline around Times Square, New York."

**🤖 AI Agent:**
> Isoline calculation finished. Based on current local routing systems, the GeoJSON geometry covers exactly the 15-minute vehicular reach extending roughly 1.8 miles outwards, factoring one-way routes. I am outputting the boundary format payload here.


## Installation & Usage

To install and use the **CARTO** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/carto](https://vinkius.com/mcp/carto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
