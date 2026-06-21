# Gobierno Abierto Valencia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gobierno-abierto-valencia)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gobierno-abierto-valencia-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gobierno-abierto-valencia-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access Valencia's Open Data portal to query datasets, resources, and public records directly from your AI agent.

## Description
Connect to the **Valencia Open Data portal (Gobierno Abierto)** to explore public datasets, groups, and specific resource data through natural conversation.

### What you can do

- **Datasets & Packages** — List all available public datasets and fetch detailed metadata for specific ones using their name or ID.
- **Resource Inspection** — Access specific file metadata, formats, and descriptions within a dataset to understand the available data structures.
- **Data Search** — Query actual records inside a resource's datastore with powerful filtering, search queries, and pagination.
- **Categories & Groups** — Browse datasets by organizational groups or thematic categories to find relevant information faster.

### How it works

1. Subscribe to this server
2. Enter your Valencia Open Data API Key (if required for specific datasets)
3. Start querying public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and inspect public datasets without manual browsing
- **Developers** — integrate real-time city data into applications by testing queries via AI
- **Citizens & Researchers** — explore municipal transparency data and public records through simple questions


## Available Tools
- **search_datastore**: Search for data within a specific resource
- **list_groups**: List dataset groups (categories)
- **show_package**: Get metadata for a specific dataset
- **list_packages**: List all dataset names
- **show_resource**: Get metadata for a specific resource


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gobierno Abierto Valencia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available datasets in the Valencia portal."

**🤖 AI Agent:**
> I've retrieved the list of datasets. There are several available, including 'Tráfico', 'EMT Valencia', and 'Presupuestos Municipales'. Which one would you like to explore?

---

**👤 You:**
> "Search for 'bicis' records in resource ID 456."

**🤖 AI Agent:**
> Searching the datastore... I found 10 records matching 'bicis'. These include real-time station availability and location data. Would you like to see the specific coordinates?

---

**👤 You:**
> "Show me the details for the dataset 'EMT Valencia'."

**🤖 AI Agent:**
> Fetching metadata for 'EMT Valencia'... This dataset contains real-time bus information, routes, and schedules. It includes 5 resources (CSV, JSON, and GeoJSON formats).


## Installation & Usage

To install and use the **Gobierno Abierto Valencia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gobierno-abierto-valencia](https://vinkius.com/mcp/gobierno-abierto-valencia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
