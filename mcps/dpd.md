# DPD MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dpd)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dpd-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dpd-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Streamline your logistics and shipping with DPD.

## Description
This MCP server integrates DPD services, allowing you to create shipments, track parcel statuses, and find nearby pickup points. It's designed for businesses that need to automate their shipping workflows efficiently.


## Available Tools
- **cancel_shipment**: Cancel an existing DPD shipment
- **create_shipment**: Provide shipment data as a JSON string.

Create a new shipment and generate parcel numbers/labels
- **find_parcelshop**: Search for DPD Pickup points (ParcelShops) near a location
- **get_labels**: Retrieve the labels for a specific shipment
- **get_manifest**: Generate or retrieve a manifest for a shipment
- **get_parcel_status**: Retrieve the tracking status for a specific parcel number
- **get_shipment_status**: Get the current status and tracking history of a shipment
- **list_countries**: List supported countries for DPD shipping
- **list_products**: List available DPD products and services
- **list_shipments**: Supports filtering by date or status. Provide filters as a JSON string.

List recent shipments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DPD** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of parcel 123456789."

**🤖 AI Agent:**
> I'm checking the current status for you.

---

**👤 You:**
> "Find DPD pickup points in Berlin."

**🤖 AI Agent:**
> Searching for nearby parcel shops...

---

**👤 You:**
> "Create a shipment from London to Paris."

**🤖 AI Agent:**
> Let's set up the shipment details.


## Installation & Usage

To install and use the **DPD** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dpd](https://vinkius.com/mcp/dpd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
