# EOSDA Agriculture Satellite Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eosda-agriculture-satellite-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eosda-agriculture-satellite-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eosda-agriculture-satellite-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Precision agriculture satellite intelligence — access NDVI, soil moisture, and crop health via AI.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EOSDA Agriculture Satellite Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find Sentinel-2 images for my farm from the last month."

**🤖 AI Agent:**
> Searching Sentinel-2 dataset for the specified date range... I found 3 cloud-free scenes. Shall I provide the scene IDs and download links for them?

---

**👤 You:**
> "Calculate the NDVI for this area: [GeoJSON coords]."

**🤖 AI Agent:**
> Initiating NDVI vegetation task for your area of interest... The task has been created with ID `task_123`. I will monitor the status and let you know once the result is ready.

---

**👤 You:**
> "What is the resolution of Landsat 8 satellite data?"

**🤖 AI Agent:**
> Landsat 8 provides high-quality imagery with a spatial resolution of 30 meters for most bands. It has a revisit time of approximately 16 days.


## Installation & Usage

To install and use the **EOSDA Agriculture Satellite Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eosda-agriculture-satellite-data](https://vinkius.com/mcp/eosda-agriculture-satellite-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
