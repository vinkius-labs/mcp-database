# DoorLoop MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doorloop)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/doorloop-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/doorloop-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage rental properties, collect rent online, screen tenants, and handle maintenance requests from one landlord platform.

## Description
Connect your **DoorLoop** account to any AI agent and take full control of your rental portfolio and real estate operations through natural conversation.

### What you can do

- **Property Orchestration** — List and manage your entire real estate portfolio programmatically, including retrieving detailed metadata for properties and individual units
- **Tenant & Lease Lifecycle** — Access complete tenant profiles and monitor active lease agreements to maintain high-fidelity records of your occupants
- **Maintenance Architecture** — Monitor maintenance requests and programmatically create new work orders to coordinate repairs and service vendors efficiently
- **Lead & Prospecting** — Retrieve directories of potential tenants (leads) to streamline your vacancy filling and marketing workflows
- **Financial Visibility** — Access summarized rent roll reports and vendor directories directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from DoorLoop (Settings > Integrations)
3. Start managing your rental business from Claude, Cursor, or any MCP client

No more manual toggling between unit lists or digging through maintenance logs. Your AI acts as your dedicated property operations and lease coordinator.

### Who is this for?

- **Property Managers** — instantly retrieve tenant contact info and check unit availability using natural language commands
- **Maintenance Coordinators** — track work order status and dispatch vendors without leaving your communication tools
- **Real Estate Investors** — monitor portfolio performance and rent roll reports through simple AI queries


## Available Tools
- **create_work_order**: Requires subject and unit/property IDs.

Create a new maintenance work order
- **get_lease_details**: Get details for a specific lease
- **get_property_details**: Get details for a specific property
- **get_rent_roll_report**: Get the current rent roll report
- **get_tenant_details**: Get details for a specific tenant
- **list_leases**: List all lease agreements
- **list_properties**: List all properties
- **list_prospects**: List prospective tenants
- **list_tenants**: List all tenants
- **list_units**: Can be filtered by property ID.

List all rental units
- **list_vendors**: List all service vendors
- **list_work_orders**: List all maintenance work orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DoorLoop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all properties and their IDs in my DoorLoop account."

**🤖 AI Agent:**
> I've retrieved your portfolio. You have 3 active properties: 'Sunset Apartments' (ID: prop_1), 'Palm Villas' (ID: prop_2), and 'Grand Plaza'. Which one should I list the units for?

---

**👤 You:**
> "Show me the maintenance requests for 'Sunset Apartments' (ID: prop_1)."

**🤖 AI Agent:**
> Scanning work orders... I found 2 active requests for Sunset Apartments: 'Leaking Faucet' in Unit 102 and 'HVAC Check' in Unit 304. Would you like the full details for either of these?

---

**👤 You:**
> "Get the rent roll report for all active units."

**🤖 AI Agent:**
> Fetching report... Your current rent roll shows 15 active leases with a total monthly revenue of $22,500. Average rent is $1,500 per unit. I can break this down by property if needed.


## Installation & Usage

To install and use the **DoorLoop** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doorloop](https://vinkius.com/mcp/doorloop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
