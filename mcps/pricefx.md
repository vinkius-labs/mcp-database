# Pricefx MCP Server

Equip your AI with advanced enterprise CPQ capabilities — fetch products, manage customers, and generate automated pricing quotes directly via chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pricefx)

## Overview
**Category:** erp-operations
**Tools Count:** 10

## Description
Harness the power of **Pricefx**, the premier Cloud Pricing Optimization platform, by coupling it directly to your LLM agents. Empower your AI to navigate vast B2B catalogs, securely read customer pricing grids, and orchestrate automated Quote generation (CPQ) instantaneously via natural language prompts.

### What you can do

- **Live Catalog & Pricing** — Search deep into the `fetch_products` logic to find base SKUs, and evaluate their explicit Price Math limits via `get_product`
- **CRM & Account Rules** — Query your partition tracing active CRM records via `fetch_customers`, or force new structures dynamically (`create_customer`)
- **Quote Engine (CPQ)** — Ask the AI to build dynamic Quotes on the fly (`create_quote`) calculating complex arrays, or trace why an exist Quote ID failed approval (`get_quote`)
- **Seamless Deletion** — Obliterate drafted quotes matching strict constraints from your Partition without accessing the Gateway (`delete_quote`)

### How it works

1. Subscribe to this MCP server
2. Provide your Pricefx Cluster, Partition Name, and active JWT Token
3. Engage Claude, Cursor, or any compatible client to navigate the Pricing Engine natively

Forget executing long, structured JSON payloads through Postman. Just tell your AI: 'Create a new Quote for Customer XYZ with Product 123'. The agent handles the structural formatting and API syntax inherently.

### Who is this for?

- **Pricing Managers** — instantly check live Price Grids or simulate logic without waiting for heavy partition dashboards to load
- **Backend Devs** — test dynamic JSON payloads for Quote generation interacting intuitively to build headless frontends
- **Sales Engineers** — quickly pull the math trace behind a specific Quote ID during high-pressure B2B negotiations


## Available Tools
- **create_customer**: Ensure JSON format is robust.

Provision a highly-available JSON Payload generating hard Customer bindings
- **create_quote**: Retrieve the exact structural matching verifying CPQ Generation
- **delete_quote**: Irreversibly vaporize explicit validations extracting rich Churn flags
- **fetch_customers**: Identify bounded CRM records inside the Headless Pricefx Platform
- **fetch_products**: Enumerate explicitly attached structured rules exporting active pricing Catalog
- **fetch_quotes**: Identify precise active arrays spanning native Gateway auth
- **get_customer**: Perform structural extraction of properties driving active Account logic
- **get_product**: Retrieve explicit Cloud logging tracing explicit Product limits
- **get_quote**: Dispatch an automated validation check routing explicit Quote history
- **update_customer**: Provide bulk bounds strictly formatted.

Inspect deep internal arrays mitigating specific Plan Math


## Installation & Usage

To install and use the **Pricefx** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pricefx](https://vinkius.com/mcp/pricefx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
