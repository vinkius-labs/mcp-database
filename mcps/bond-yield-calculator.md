# Bond Yield Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bond-yield-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bond-yield-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bond-yield-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate YTM, Current Yield, and interest rate sensitivity for fixed-income bonds.

## Description
This MCP server provides advanced financial engineering tools to value fixed-income instruments. Using the `get_bond_yield_metrics` tool, you can determine the Yield to Maturity (YTM) and Current Yield based on market price, face value, and coupon rates. It also calculates risk metrics like Modified Duration and Convexity, and estimates price volatility for various interest rate shifts (1bp, 25bp, and 100bp). Perfect for bond traders and analysts needing precise sensitivity analysis.


## Available Tools
- **get_bond_yield_metrics**: Calculate Yield to Maturity (YTM), Current Yield, and interest rate sensitivity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bond Yield Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected annual return profile of a bond with a market price of 950, face value of 1000, coupon rate of 5%, semi-annual payments, and 5 years to maturity?"

**🤖 AI Agent:**
> The Yield to Maturity (YTM) is approximately 6.17% and the Current Yield is 5.26%.

---

**👤 You:**
> "How much risk does a bond with market price 980, face value 1000, coupon rate 4%, annual payments, and 10 years to maturity carry regarding interest rate movements?"

**🤖 AI Agent:**
> The bond has a Modified Duration of approximately 8.25 and a Convexity of 75.4.

---

**👤 You:**
> "How will the bond's price change if interest rates shift by 100 basis points? (Price: 950, Face: 1000, Coupon: 6%, Frequency: 2, Maturity: 3)"

**🤖 AI Agent:**
> A 100 basis point increase in rates is estimated to cause a price decrease of approximately 4.5%.


## Installation & Usage

To install and use the **Bond Yield Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bond-yield-calculator](https://vinkius.com/mcp/bond-yield-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
