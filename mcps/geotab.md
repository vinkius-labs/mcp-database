# Geotab MCP Server

Automate fleet management via Geotab — manage devices, track trips, and monitor vehicle diagnostics directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/geotab)

## Overview
**Category:** iot-hardware
**Tools Count:** 7

## Description
Connect your **MyGeotab** account to any AI agent to streamline your telematics and fleet operations through natural conversation.

### What you can do

- **Entity Management** — Retrieve, create, or update Devices, Users, Zones, and Rules using `get_entity`, `add_entity`, and `set_entity`.
- **Real-time Data Feeds** — Use `get_feed` for high-volume synchronization of LogRecords, StatusData, and FaultData.
- **Trip & Exception Tracking** — Query historical Trips and ExceptionEvents to analyze fleet behavior and safety compliance.
- **Batch Operations** — Execute multiple API calls in a single request with `execute_multi_call` for maximum efficiency.
- **Quick Auditing** — Get instant counts of specific records using `get_count_of` without downloading entire datasets.

### How it works

1. Subscribe to this server
2. Provide your Geotab credentials (Server, Database, Username, and Password)
3. Start managing your fleet from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fleet Managers** — monitor vehicle health and trip history without manual report generation.
- **Developers** — integrate telematics data into workflows using natural language instead of complex SDK calls.
- **Operations Teams** — quickly audit user access and device status across large databases.


## Available Tools
- **add_entity**: Provide the full entity JSON object.

Creates a new entity in the database
- **get_count_of**: Returns the number of entities matching a search
- **get_feed**: Returns up to 50,000 records and a toVersion token for the next call.

Continuously retrieves new or updated data (incremental polling)
- **get_entity**: Retrieves a list of entities based on search criteria
- **execute_multi_call**: Provide a JSON array of call objects, each containing a "method" and "params".

Executes multiple API calls in a single HTTP request
- **remove_entity**: Deletes an entity from the database
- **set_entity**: The entity JSON must include the ID of the record being updated.

Updates an existing entity


## Installation & Usage

To install and use the **Geotab** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geotab](https://vinkius.com/mcp/geotab)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
