# EOSDA Agriculture Satellite Data MCP Server

Precision agriculture satellite intelligence — access NDVI, soil moisture, and crop health via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/eosda-agriculture-satellite-data)

## Overview
**Category:** the-unthinkable
**Tools Count:** 6

## Description
Empower your AI agent with cutting-edge remote sensing capabilities via the **EOSDA Agriculture** MCP server. This integration provides instant access to high-resolution satellite data from Sentinel and Landsat missions, specifically processed for precision farming. Your agent can search for imagery across global datasets, calculate vegetation indices like NDVI, EVI, and MSAVI, and monitor soil moisture trends over time. Whether you are optimizing fertilizer application, auditing crop health, or monitoring land use, your agent acts as a dedicated agronomist and remote sensing specialist through natural conversation.

### What you can do

- **Satellite Imagery Search** — Search Sentinel-2, Landsat 8/9, and MODIS datasets by date and area of interest.
- **Vegetation Indices** — Trigger processing tasks for NDVI (health), EVI (biomass), and other critical indices.
- **Health Monitoring** — Retrieve processed results to identify areas of stress or high productivity in fields.
- **Dataset Intelligence** — Access technical specs for available satellites including resolution and revisit times.
- **AOI Analysis** — Input GeoJSON areas of interest to get localized intelligence for specific farms or regions.

### How it works

1. Subscribe to this server
2. Enter your EOSDA API Key (from EOS Data Analytics dashboard)
3. Start managing your precision agriculture data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agronomists & Farm Managers** — monitor field performance and crop health without manual site visits.
- **Ag-Tech Developers** — integrate remote sensing data into custom farming applications.
- **Sustainability Officers** — track land use changes and vegetation trends over large geographic areas.
- **Researchers** — access historical and near real-time satellite data for agricultural studies.


## Available Tools
- **search_dataset**: ) within a date range and optional area of interest. Returns scene IDs, dates, cloud cover percentages and download URLs. Use get_available_datasets to see all dataset options.

Search satellite imagery for a specific dataset
- **search_multi_dataset**: g. Sentinel-2 and Landsat 8 together). Returns scenes from all requested datasets within the date range and area of interest.

Search satellite imagery across multiple datasets
- **create_vegetation_task**: ) for a specific area of interest. Returns a task ID that can be used with get_task_result to retrieve results. Use get_available_indices to see all available index types.

Create a vegetation index calculation task (NDVI, EVI, etc.)
- **get_available_datasets**: Use these dataset IDs for search_dataset and create_vegetation_task.

Get list of available satellite datasets
- **get_available_indices**: Use these index types with create_vegetation_task.

Get list of available vegetation indices
- **get_task_result**: Returns the processed vegetation index data, download URLs and status.

Get the result of a vegetation index task


## Installation & Usage

To install and use the **EOSDA Agriculture Satellite Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eosda-agriculture-satellite-data](https://vinkius.com/mcp/eosda-agriculture-satellite-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
