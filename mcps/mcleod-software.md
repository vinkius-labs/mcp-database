# McLeod Software MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mcleod-software)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mcleod-software-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mcleod-software-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Transportation management via McLeod Software — manage orders, dispatches, and carriers.

## Description
Connect your **McLeod Software** LoadMaster or PowerBroker instance to any AI agent and take full control of your transportation management through natural conversation.

### What you can do

- **Order Management** — List all orders, search by term, and fetch detailed shipment metadata
- **Dispatch Orchestration** — Monitor active dispatches, movements, and driver assignments in real-time
- **Entity Management** — List and inspect master records for customers, carriers, and company drivers
- **Operational Visibility** — Access stop-level details for movements and detailed dispatch configurations

### How it works

1. Subscribe to this server
2. Enter your McLeod Base URL, Client ID, Client Secret, and Company ID
3. Start managing your logistics operations from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_dispatch_details**: Get details for a specific dispatch
- **get_order**: Get details for a specific order
- **list_carriers**: List master carrier records
- **list_customers**: List master customer records
- **list_dispatches**: List dispatch assignments
- **list_drivers**: List all drivers
- **list_movements**: List truckload movements
- **list_orders**: List all transportation orders
- **list_stops**: List stops for a movement
- **search_orders**: Search for orders by term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **McLeod Software** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 transportation orders."

**🤖 AI Agent:**
> Retrieving orders... I found several orders including ORD-98765 for TechCorp and ORD-98764 for GlobalLogistics.

---

**👤 You:**
> "Search for orders related to 'Chicago'."

**🤖 AI Agent:**
> Searching... I identified 3 orders with routes starting or ending in Chicago.

---

**👤 You:**
> "What is the status of dispatch assignment ID 555?"

**🤖 AI Agent:**
> Inspecting dispatch... Assignment 555 is currently 'In Transit', driven by John Smith.


## Installation & Usage

To install and use the **McLeod Software** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mcleod-software](https://vinkius.com/mcp/mcleod-software)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
