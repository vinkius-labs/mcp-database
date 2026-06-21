# Metrc MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/metrc)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/metrc-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/metrc-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Cannabis track-and-trace via Metrc — track facilities, items, plants, and harvests.

## Description
Connect your **Metrc** account to any AI agent and take full control of your cannabis track-and-trace compliance through natural conversation.

### What you can do

- **Facility Oversight** — List all licensed facilities and fetch detailed metadata for your operations
- **Inventory Tracking** — Retrieve active items, strains, and inventory packages with real-time status visibility
- **Supply Chain Management** — Monitor plant life cycles, harvest batches, and incoming inventory transfers securely
- **Compliance Auditing** — List active sales receipts and verify unit of measure configurations
- **Detailed Inspection** — Fetch comprehensive metadata for individual packages and state-specific license configurations

### How it works

1. Subscribe to this server
2. Enter your state-specific Metrc Base URL, Integrator Key, and User Key
3. Start managing your compliance data from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_package_details**: Get details for a specific package
- **get_unit_of_measures**: g. Grams, Ounces).

List all units of measure
- **list_facilities**: List all licensed facilities
- **list_active_harvests**: List active harvests for a facility
- **list_active_items**: List active items for a facility
- **list_active_packages**: List active packages for a facility
- **list_tracked_plants**: List tracked plants for a facility
- **list_active_sales**: List active sales receipts
- **list_active_strains**: List active strains for a facility
- **list_incoming_transfers**: List incoming inventory transfers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metrc** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active facilities associated with my Metrc account."

**🤖 AI Agent:**
> Retrieving facilities... I found 2 licensed facilities: 'Green Valley Cultivation' and 'Downtown Distribution Center'.

---

**👤 You:**
> "Show active inventory packages for license 'LIC-12345'."

**🤖 AI Agent:**
> Querying inventory... I identified 15 active packages, including 10 units of 'Blue Dream' flower and 5 units of 'OG Kush' concentrates.

---

**👤 You:**
> "Get details for package label 'ABCDEFG1234567'."

**🤖 AI Agent:**
> Inspecting package... Label 'ABCDEFG1234567' contains 500g of bulk flower, currently in 'Active' status at your primary facility.


## Installation & Usage

To install and use the **Metrc** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metrc](https://vinkius.com/mcp/metrc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
