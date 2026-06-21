# Tax Loss Harvesting Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tax-loss-harvesting-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tax-loss-harvesting-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tax-loss-harvesting-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the financial benefits and tax savings from harvesting capital losses.

## Description
This MCP server provides specialized tools to calculate the economic impact of tax-loss harvesting. Use `evaluate_harvesting_opportunity` to determine avoided taxes and net savings after reinvestment friction. You can also use `get_wash_sale_window` to check compliance periods for different jurisdictions like the USA or Germany, and `retrieve_tax_rate_by_jurisdiction` to find applicable capital gains rates based on your location and income band.


## Available Tools
- **evaluate_harvesting_opportunity**: Calculates the potential tax benefits and net economic impact of harvesting losses
- **retrieve_tax_rate_by_jurisdiction**: Retrieves the correct capital gains percentage based on jurisdiction and income band
- **get_wash_sale_window**: Determines the regulatory window for wash sale compliance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tax Loss Harvesting Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my tax savings if I have a loss of $5000 with a 15% tax rate and $50 in fees."

**🤖 AI Agent:**
> The total avoided tax is $750.00, and your net savings after the $50.00 friction cost is $700.00.

---

**👤 You:**
> "What is the wash sale window in Germany?"

**🤖 AI Agent:**
> The wash sale window for Germany is 0 days.

---

**👤 You:**
> "What capital gains rate applies to me in the USA if I am in the medium income band?"

**🤖 AI Agent:**
> The applicable capital gains tax rate for the medium income band in the USA is 15%.


## Installation & Usage

To install and use the **Tax Loss Harvesting Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tax-loss-harvesting-calculator](https://vinkius.com/mcp/tax-loss-harvesting-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
