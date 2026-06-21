# FishBase MCP Server

Access the world's largest database of fish species. Query common names, database versions, and technical documentation for FishBase and SeaLifeBase.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fishbase)

## Overview
**Category:** databases
**Tools Count:** 5

## Description
Connect to **FishBase** and **SeaLifeBase**, the premier global information systems on fishes and marine organisms. This MCP server allows AI agents to query extensive biological data, common names, and database schema documentation directly.

### What you can do

- **Species Common Names** — Search and list common names of fishes with support for pagination and species filtering using `list_comnames`.
- **Database Versions** — Access different versions of the FishBase/SeaLifeBase databases to track historical records via `get_versions`.
- **Technical Documentation** — Retrieve metadata and documentation for specific database tables to understand the underlying schema with `get_docs_by_table`.
- **Dual Database Support** — Seamlessly switch between FishBase and SeaLifeBase using a simple toggle in any query.
- **API Health Monitoring** — Check the real-time status and heartbeat of the API to ensure connectivity.

### How it works

1. Subscribe to this server
2. Enter your FishBase API Key (if required by your provider)
3. Start exploring ichthyological data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marine Biologists & Researchers** — Quickly verify species data and common names across different regions.
- **Data Scientists** — Understand the FishBase schema and available versions for large-scale data analysis.
- **Educators & Students** — Access reliable, peer-reviewed information about fish species for academic projects.


## Available Tools
- **list_comnames**: Supports pagination and field filtering.

Access common names data for fishes
- **get_docs_by_table**: Get documentation for a specific database table
- **get_docs**: Get documentation metadata for the FishBase API
- **get_heartbeat**: The root URL redirects here.

Get the current status and time of the FishBase API
- **get_versions**: g., v3, v4) which correspond to specific dates.

List available database versions


## Installation & Usage

To install and use the **FishBase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fishbase](https://vinkius.com/mcp/fishbase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
