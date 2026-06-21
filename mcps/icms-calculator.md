# ICMS Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/icms-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/icms-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/icms-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Brazilian ICMS taxes, including tax substitution (ST), tax differentials (DIFAL), and tax-inclusive base calculations.

## Description
This MCP server provides specialized tools for calculating complex Brazilian ICMS taxes. It handles the 'inside' calculation method to find grossed-up product values, calculates Tax Substitution (ICMS-ST) using MVA (Added Value Margin), determines the tax differential (DIFAL) for B2C interstate transactions, and retrieves correct interstate rates based on regional movements. Use `calculate_tax_base` for tax-inclusive bases, `calculate_icms_substitution` for ST calculations, `calculate_tax_differential` for DIFAL, and `get_interstate_rate` to identify applicable rates between Brazilian regions.


## Available Tools
- **calculate_tax_differential**: Calculates the DIFAL amount for B2C interstate operations
- **calculate_icms_substitution**: Calculates the amount of ICMS-ST (Tax Substitution) to be collected
- **calculate_tax_base**: Calculates the grossed-up product value using the "inside" calculation method
- **get_interstate_rate**: Retrieves the correct interstate tax rate based on origin and destination regions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ICMS Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the tax base for a product worth 100.00 with an 18% tax rate."

**🤖 AI Agent:**
> The `calculate_tax_base` tool would return a tax base of approximately 121.95 and a tax amount of 21.95.

---

**👤 You:**
> "What is the interstate rate for a shipment from Southeast to North region?"

**🤖 AI Agent:**
> Using `get_interstate_rate` with origin 'Southeast' and destination 'North', the tool returns a rate of 7%.

---

**👤 You:**
> "Calculate DIFAL for a product worth 500.00, with an interstate rate of 12% and destination internal rate of 18%."

**🤖 AI Agent:**
> The `calculate_tax_differential` tool calculates a DIFAL amount of 30.00.


## Installation & Usage

To install and use the **ICMS Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/icms-calculator](https://vinkius.com/mcp/icms-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
