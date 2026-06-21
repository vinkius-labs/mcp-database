# Cloverly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloverly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cloverly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cloverly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Offset carbon emissions at the point of transaction by purchasing verified carbon credits for shipments, rides, and purchases.

## Description
Connect your **Cloverly** account to any AI agent and take full control of your sustainability initiatives and automated carbon management workflows through natural conversation.

### What you can do

- **Footprint Orchestration** — Calculate real-time carbon footprint estimates for diverse activities including logistics (freight, shipping), travel (flights, vehicles), and energy usage programmatically
- **Automated Offset Ingestion** — Execute the purchase of carbon offsets based on specific activity estimates or fixed currency amounts to maintain high-fidelity sustainability compliance
- **Project Intelligence** — Access your complete directory of high-impact environmental projects (wind, solar, reforestation) to understand the source of your offsets directly through your agent
- **Transaction Monitoring** — Programmatically track your purchase history and retrieve detailed metadata, certificates, and receipts for operational and regulatory reporting
- **Sustainability Visibility** — Check the status of individual offset purchases and monitor account-level metadata to perfectly coordinate your organization's climate action

### How it works

1. Subscribe to this server
2. Retrieve your **Public and Private API Keys** from the Cloverly dashboard (Settings > API)
3. Start offsetting your business operations from Claude, Cursor, or any MCP client

No more manual footprint spreadsheets or searching for carbon certificates in the portal. Your AI acts as your dedicated sustainability engineer and climate coordinator.

### Who is this for?

- **Sustainability Managers** — instantly calculate project footprints and manage offset portfolios using natural language commands
- **Logistics & E-commerce Ops** — automate carbon offsetting for every shipment and monitor environmental impact without leaving your workspace
- **Growth Engineers** — integrate real-time carbon calculation and purchase features into custom internal tools through simple AI queries


## Available Tools
- **check_cloverly_status**: Verify connectivity
- **create_estimate**: Create a carbon estimate
- **create_purchase**: Purchase carbon offsets
- **get_account**: Get account info
- **get_estimate**: Get estimate details
- **get_impact_by_type**: Get impact by type
- **get_impact_summary**: Get impact summary
- **get_project**: Get project details
- **get_purchase**: Get purchase details
- **list_estimates**: List estimates
- **list_projects**: List offset projects
- **list_purchases**: List purchases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloverly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the carbon footprint for a 10kg shipment from Berlin to Paris."

**🤖 AI Agent:**
> Footprint calculated! Shipping your 10kg package results in approximately 1,200g of CO2 emissions. The cost to offset this is $0.15 USD. Shall I proceed with the purchase using your default project?

---

**👤 You:**
> "List the available reforestation projects on Cloverly."

**🤖 AI Agent:**
> I've retrieved the project directory. Currently, you can support: 'Amazon Rainforest Protection' (ID: prj_123), 'US Heritage Forests', and 'Mangrove Restoration'. Which one would you like more details on?

---

**👤 You:**
> "Show the status of my latest offset purchase 'pur_456'."

**🤖 AI Agent:**
> Monitoring purchase... Offset pur_456 is 'Confirmed'. I've retrieved your high-fidelity carbon certificate. You can view the digital receipt here: [receipt_url]. Need help with another sustainability report?


## Installation & Usage

To install and use the **Cloverly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloverly](https://vinkius.com/mcp/cloverly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
