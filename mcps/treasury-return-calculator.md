# Treasury Return Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/treasury-return-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/treasury-return-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/treasury-return-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate fair price, YTM, and inflation-adjusted returns for US Treasuries, UK Gilts, and German Bunds.

## Description
This MCP server provides specialized financial tools to value sovereign debt instruments. Use `calculate_bond_valuation` to determine the fair market price and annualized total return (YTM) for bonds like US T-Bills, T-Notes, or German Bunds based on current market yields. The `calculate_inflation_adjusted_return` tool allows you to assess purchasing power preservation by adjusting nominal returns against expected inflation rates. Additionally, use `calculate_currency_equivalent_yield` to evaluate the yield of a foreign bond when converted into a target currency, accounting for exchange rate impacts.


## Available Tools
- **calculate_bond_valuation**: Calculate fair market price and annualized total return (YTM) of a bond
- **calculate_currency_equivalent_yield**: Evaluate the yield of a foreign sovereign bond in a target currency
- **calculate_inflation_adjusted_return**: Assess purchasing power preservation by adjusting nominal return for inflation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Treasury Return Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the fair price of a US T-Note with a 3% coupon, 2 years to maturity, and a 4% market yield?"

**🤖 AI Agent:**
> The calculated fair price for the bond is 97.15.

---

**👤 You:**
> "If my bond has a 5% nominal return and inflation is expected to be 2%, what is my real return?"

**🤖 AI Agent:**
> Your inflation-adjusted real return is approximately 2.94%.

---

**👤 You:**
> "Calculate the yield of a GBP bond with 4% yield if the USD/GBP exchange rate is 1.25."

**🤖 AI Agent:**
> The converted yield in the target currency is 4.0%.


## Installation & Usage

To install and use the **Treasury Return Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/treasury-return-calculator](https://vinkius.com/mcp/treasury-return-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
