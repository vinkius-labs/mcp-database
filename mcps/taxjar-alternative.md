# TaxJar MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/taxjar-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/taxjar-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/taxjar-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Calculate, collect, and remit sales tax automatically across every US state and jurisdiction with real-time rate accuracy.

## Description
Connect your **TaxJar** sales tax automation account to any AI agent and simplify how you calculate tax rates, manage jurisdictional nexus, and monitor order compliance through natural conversation.

### What you can do

- **Precise Tax Calculation** — Calculate real-time sales tax for orders based on specific destination addresses and product categories.
- **Rate Lookup** — Retrieve general sales tax rates for any ZIP code or city to estimate costs instantly.
- **Nexus Management** — List and monitor regions where your business has a sales tax nexus to ensure compliance.
- **Transaction Oversight** — Record, update, and manage sales order and refund transactions for automated reporting.
- **Address Validation** — Verify street addresses to ensure highly accurate tax jurisdiction identification.
- **Product Categorization** — List TaxJar product categories and codes to apply correct tax exemptions and rates.

### How it works

1. Subscribe to this server
2. Enter your TaxJar API Token (found in your account settings)
3. Start managing your sales tax compliance from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Managers** — quickly calculate taxes for custom orders and check nexus status via simple AI commands.
- **Finance & Accounting Teams** — monitor transaction history and verify sales tax collected directly from the workspace.
- **Ops & Logistics** — validate shipping addresses and ensure correct product categorization via the AI assistant.


## Available Tools
- **calculate_sales_tax**: Calculate order tax
- **create_tax_order**: Record order transaction
- **create_tax_refund**: Record refund
- **delete_tax_order**: Remove order record
- **get_tax_account**: Get API status
- **get_tax_order**: Get order details
- **get_tax_rates**: Get rates by ZIP
- **list_tax_categories**: List product types
- **list_nexus_regions**: List tax nexus
- **list_tax_orders**: List order transactions
- **update_tax_order**: Modify order record
- **validate_tax_address**: Verify address for tax


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TaxJar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate sales tax for a $150 order to NY 10001, USA."

**🤖 AI Agent:**
> I've calculated the tax. For a $150.00 order to New York (10001), the total sales tax is $13.31 (8.875%). The total amount including tax would be $163.31. Would you like to log this transaction?

---

**👤 You:**
> "Show me all regions where I have a tax nexus."

**🤖 AI Agent:**
> Retrieving nexus data... You currently have active sales tax nexus in 3 regions: California (CA), Florida (FL), and New York (NY). Shall I check the tax rates for any of these states?

---

**👤 You:**
> "Find the tax rate for ZIP code 90210."

**🤖 AI Agent:**
> The sales tax rate for Beverly Hills (90210, CA) is currently 9.5%. This includes a state rate of 6%, a county rate of 0.25%, and a local rate of 3.25%.


## Installation & Usage

To install and use the **TaxJar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/taxjar-alternative](https://vinkius.com/mcp/taxjar-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
