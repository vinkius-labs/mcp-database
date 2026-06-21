# Smarty MCP Server

Equip your AI with enterprise-grade location intelligence to validate, autocomplete, and extract US or International addresses instantly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/smarty)

## Overview
**Category:** developer-tools
**Tools Count:** 7

## Description
Connect your **Smarty** account to any AI agent and empower your team to sanitize raw address data, query ZIP codes, and format global street locations securely. Interact with powerful geospatial and mailing validation APIs through natural language without writing a single line of custom script.

### What you can do

- **Address Validation (USA/Intl)** — Effortlessly clean and verify messy user inputs calling `validate_us_address`, returning the Delivery Point Validation (DPV)
- **Text Extraction** — Feed your AI unformatted text like emails or notes and run `extract_addresses` to intelligently isolate real physical addresses
- **Autocompletion Tests** — Interrogate the AI dynamically with partial street names using the `autocomplete_us_address` algorithm
- **ZIP Code Checks** — Validate specific 5-digit postal zones using `verify_zip_code` to retrieve associated municipal limits

### How it works

1. Subscribe to this server
2. Enter your Smarty Auth ID and Auth Token
3. Start using Claude, Cursor, or any MCP-compatible client to query your geospatial APIs directly

Stop manually typing test addresses into the Smarty sandbox or setting up Postman. Your AI agent can validate address inputs right inside your coding or chat interface.

### Who is this for?

- **E-Commerce Devs** — test the viability of formatting algorithms by parsing complex address lines dynamically in your IDE
- **Data Engineers** — upload raw customer data lists to your AI and have it extract valid postal locations sequentially
- **Logistics Teams** — quickly verify delivery endpoints for complex multi-unit apartment addresses internally


## Available Tools
- **autocomplete_intl_address**: Predictive autocomplete for international addresses
- **autocomplete_us_address**: Predictive autocomplete for US addresses
- **extract_addresses**: g., emails, documents) and find valid addresses.

Extracts physical addresses from raw text
- **get_account_info**: Retrieves Smarty account information
- **validate_intl_address**: Requires at least the address line and country.

Validates and geocodes an international street address
- **validate_us_address**: Returns delivery point validation (DPV) status and coordinates.

Validates and geocodes a US street address
- **verify_zip_code**: Verifies a ZIP code and returns associated cities and states


## Installation & Usage

To install and use the **Smarty** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smarty](https://vinkius.com/mcp/smarty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
