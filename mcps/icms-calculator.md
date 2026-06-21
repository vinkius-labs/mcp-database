# ICMS Calculator MCP Server

Calculate Brazilian ICMS taxes, including tax substitution (ST), tax differentials (DIFAL), and tax-inclusive base calculations.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/icms-calculator)

## Overview
**Category:** finance
**Tools Count:** 4

## Description
This MCP server provides specialized tools for calculating complex Brazilian ICMS taxes. It handles the 'inside' calculation method to find grossed-up product values, calculates Tax Substitution (ICMS-ST) using MVA (Added Value Margin), determines the tax differential (DIFAL) for B2C interstate transactions, and retrieves correct interstate rates based on regional movements. Use `calculate_tax_base` for tax-inclusive bases, `calculate_icms_substitution` for ST calculations, `calculate_tax_differential` for DIFAL, and `get_interstate_rate` to identify applicable rates between Brazilian regions.


## Available Tools
- **calculate_tax_differential**: Calculates the DIFAL amount for B2C interstate operations
- **calculate_icms_substitution**: Calculates the amount of ICMS-ST (Tax Substitution) to be collected
- **calculate_tax_base**: Calculates the grossed-up product value using the "inside" calculation method
- **get_interstate_rate**: Retrieves the correct interstate tax rate based on origin and destination regions


## Installation & Usage

To install and use the **ICMS Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/icms-calculator](https://vinkius.com/mcp/icms-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
