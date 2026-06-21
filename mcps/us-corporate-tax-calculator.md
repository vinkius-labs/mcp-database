# US Corporate Tax Calculator MCP Server

Estimate US federal and state corporate income taxes, providing comparative analysis between C-Corp, S-Corp, and LLC structures.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/us-corporate-tax-calculator)

## Overview
**Category:** finance
**Tools Count:** 3

## Description
This MCP server provides a specialized calculation engine for estimating US corporate tax liabilities. It allows AI agents to retrieve state-specific tax rates using `get_state_tax_rate`, calculate detailed federal and state tax breakdowns with `calculate_tax_liability`, and perform complex comparative analyses between different business entities like C-Corp, S-Corp, and LLC via `compare_business_structures`. The tool accounts for the 21% flat federal rate and applies hardcoded state-level corporate income tax rates to provide an accurate effective tax rate estimation.


## Available Tools
- **calculate_tax_liability**: Calculates the specific tax breakdown for a single profit amount in a given state
- **compare_business_structures**: Provides a side-by-side comparison of tax burdens for different business structures
- **get_state_tax_rate**: Retrieves the hardcoded corporate income tax rate for a specific US state


## Installation & Usage

To install and use the **US Corporate Tax Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-corporate-tax-calculator](https://vinkius.com/mcp/us-corporate-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
