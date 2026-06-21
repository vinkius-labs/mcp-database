# ShipEngine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shipengine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shipengine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shipengine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Compare shipping rates, print labels, and track packages across UPS, FedEx, USPS, and dozens of global carriers instantly.

## Description
Connect your **ShipEngine** account to any AI agent and take full control of your multi-carrier shipping and logistics orchestration through natural conversation. ShipEngine provides a robust platform for comparing shipping rates, validating addresses, and tracking packages, and this integration allows you to retrieve shipment metadata, generate labels, and monitor carrier details directly from your chat interface.

### What you can do

- **Rate & Shipment Orchestration** — Compare shipping rates across multiple carriers and create shipments programmatically to ensure your logistics are always optimized.
- **Label Lifecycle Management** — Generate shipping labels and retrieve detailed metadata for specific transactions directly from the AI interface.
- **Address Validation Intelligence** — Verify and validate sender and recipient addresses programmatically to ensure accurate delivery and tax calculations.
- **Tracking & Package Monitoring** — Retrieve real-time tracking information and monitor package statuses via natural language.
- **Carrier & Account Oversight** — Access carrier accounts and retrieve account profile metadata to maintain a clear overview of your shipping infrastructure.

### How it works

1. Subscribe to this server
2. Enter your ShipEngine API Key from your dashboard settings
3. Start managing your shipping operations from Claude, Cursor, or any MCP-compatible client

No more manual address checking or rate hunting. Your AI acts as a dedicated shipping clerk or logistics manager.

### Who is this for?

- **Logistics Managers** — quickly compare carrier rates and generate labels without switching apps.
- **Customer Success Teams** — automate the retrieval of package tracking statuses and validate addresses via natural conversation.
- **Developers** — integrate comprehensive multi-carrier shipping capabilities into custom AI-driven business workflows.


## Available Tools
- **create_shipping_label**: Generate shipping label
- **create_shipment_object**: Add shipment record
- **get_connection_status**: Check API health
- **get_carrier_details**: Get carrier info
- **get_label_info**: Get label metadata
- **get_shipping_rates**: Compare carrier rates
- **get_shipment_info**: Get shipment details
- **list_carriers**: List connected carriers
- **list_created_labels**: List purchased labels
- **list_shipments**: List recent shipments
- **track_package**: Check shipment status
- **validate_address**: Verify shipping address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShipEngine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this address: 123 Main St, Austin, TX 78701."

**🤖 AI Agent:**
> I've validated the address. It's a valid residential address in Austin, Texas. Would you like to check shipping rates for a package to this location?

---

**👤 You:**
> "List all active carrier accounts in my ShipEngine."

**🤖 AI Agent:**
> Retrieving carrier accounts... You have 3 active accounts: FedEx, UPS, and USPS. Would you like to see the profile metadata for any of them?

---

**👤 You:**
> "Track the shipment with ID sh_123456789."

**🤖 AI Agent:**
> Checking tracking status... Shipment sh_123456789 is currently 'Out for Delivery' via FedEx. It was last scanned at the local distribution center. Should I notify you when it's delivered?


## Installation & Usage

To install and use the **ShipEngine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shipengine](https://vinkius.com/mcp/shipengine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
