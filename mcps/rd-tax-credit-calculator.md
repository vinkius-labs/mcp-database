# R&D Tax Credit Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rd-tax-credit-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rd-tax-credit-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rd-tax-credit-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate US R&D tax credits using Regular and ASC methodologies.

## Description
This MCP server provides specialized tools to calculate United States federal R&D tax credits. It supports both the Regular Research Credit method, which calculates credit based on expenses exceeding a base amount, and the Alternative Simplified Credit (ASC) method, which uses an average of prior years' qualified research expenses. Use `calculate_regular_method_credit` for threshold-based calculations, `calculate_asc_method_credit` for historical average-based calculations, or `recommend_optimal_tax_strategy` to automatically identify the most beneficial approach for your business.


## Available Tools
- **calculate_asc_method_credit**: Determines the specific tax credit amount generated using the Alternative Simplified Credit methodology
- **recommend_optimal_tax_strategy**: Compares both methodologies to identify which approach provides the highest tax savings
- **calculate_regular_method_credit**: Returns zero if expenses do not exceed base.

Determines the specific tax credit amount generated using the Regular Research Credit methodology


## 💬 Prompt Examples

Here are some examples of how you can interact with the **R&D Tax Credit Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my regular R&D credit if my current QRE is $100,000 and my base amount is $50,000."

**🤖 AI Agent:**
> Using `calculate_regular_method_credit`, your calculated credit is $10,000 (20% of the $50,000 excess).

---

**👤 You:**
> "What is my ASC credit if my QREs for the last 3 years were $80,000, $90,000, and $100,000?"

**🤖 AI Agent:**
> Based on `calculate_asc_method_credit`, your calculated credit is $6,300 (14% of 50% of the $90,000 average).

---

**👤 You:**
> "Recommend a strategy for current QRE of $120,000, base amount of $60,000, and prior years QREs of [70000, 80000, 90000]."

**🤖 AI Agent:**
> The `recommend_optimal_tax_strategy` tool recommends the Regular method, providing a higher credit value compared to the ASC method for your data.


## Installation & Usage

To install and use the **R&D Tax Credit Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rd-tax-credit-calculator](https://vinkius.com/mcp/rd-tax-credit-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
