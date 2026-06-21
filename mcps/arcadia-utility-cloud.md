# Arcadia Utility Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arcadia-utility-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/arcadia-utility-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/arcadia-utility-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Automate utility data collection with Arcadia Utility Cloud — track accounts, bills, and usage via AI.

## Description
The **Arcadia Utility Cloud MCP Server** (formerly Urjanet) provides an advanced natural language interface for automated utility data management. Seamlessly retrieve billing data, monitor consumption patterns, and audit your utility account inventory across thousands of global providers.

### Key Capabilities

- **Automated Statement Collection** — List and retrieve metadata for all collected utility bills, including charges and periods.
- **Consumption Monitoring** — Access granular usage data for individual meters to analyze energy and resource patterns.
- **Inventory Oversight** — Manage your large-scale inventory of utility accounts and meters with ease.
- **Global Provider Support** — Interface with a vast network of electric, gas, water, and waste providers through a unified API.
- **Data Integrity** — Access verified, high-quality utility data suitable for financial and sustainability reporting.
- **Secure Integration** — Uses standard OAuth 2.0 authentication to protect your sensitive operational data.

### Who is this for?

- **Sustainability Managers** — Effortlessly gather utility data for carbon footprint calculations and ESG disclosures.
- **Accounts Payable** — Audit utility billing across large portfolios to ensure accuracy and identify savings.
- **Energy Engineers** — Retrieve meter-level data to monitor efficiency improvements and resource consumption.


## Available Tools
- **get_account_check**: Verify Arcadia Utility Cloud connection
- **get_meter_data**: Retrieve consumption and usage data for a specific meter
- **get_statement**: Get metadata for a specific statement
- **list_accounts**: List all utility accounts available in the Utility Cloud
- **list_meters**: List all utility meters tracked in the cloud
- **list_statements**: List all collected utility statements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arcadia Utility Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active utility accounts in the cloud."

**🤖 AI Agent:**
> I've retrieved your active inventory. You have 25 accounts across 5 providers, including electricity, water, and gas services.

---

**👤 You:**
> "Get consumption data for water meter 'met_12345'."

**🤖 AI Agent:**
> Retrieved usage data for meter 'met_12345'. In the last billing period, it recorded 4,500 gallons of water consumption.

---

**👤 You:**
> "Show me the latest electricity bill metadata for account ID 'acc_9988'."

**🤖 AI Agent:**
> The latest statement for account 'acc_9988' was issued on Jan 15, 2024, with total charges of $312.50.


## Installation & Usage

To install and use the **Arcadia Utility Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcadia-utility-cloud](https://vinkius.com/mcp/arcadia-utility-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
