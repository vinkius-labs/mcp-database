# Home River Group MCP Server

Connect and manage Home River Group properties, units, and residents via Entrata API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/home-river-group)

## Overview
**Category:** real-estate
**Tools Count:** 10

## Description
Empower your AI agents to interact with Home River Group's property management system. This MCP server allows listing properties, checking unit availability, managing resident information, tracking work orders, and creating leads directly through Entrata. Perfect for automating property maintenance workflows and prospect management.


## Available Tools
- **create_lead**: Submits a new lead/prospect to Home River Group
- **create_work_order**: Creates a new maintenance work order
- **get_availability**: Checks availability for units in a property
- **get_leads**: Lists sales leads and prospects
- **get_lease_info**: Retrieves detailed lease information for residents
- **get_ledgers**: Retrieves financial ledgers for residents
- **get_properties**: This is the starting point to get PropertyIDs needed for other tools. You can filter by specific property IDs or search by name in the results.

Lists properties managed by Home River Group
- **get_residents**: You can filter by propertyId to see residents of a specific building.

Lists residents across properties
- **get_units**: Requires a valid PropertyID.

Lists units for a specific property ID
- **get_work_orders**: Filtering by propertyId is highly recommended.

Lists maintenance work orders


## Installation & Usage

To install and use the **Home River Group** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/home-river-group](https://vinkius.com/mcp/home-river-group)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
