# Percentage Calculation Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/percentage-calculation-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/percentage-calculation-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/percentage-calculation-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Stop LLMs from miscalculating discounts and interest. Deterministically calculate exact percentages and relative increases.

## Description
LLMs frequently fail when applying layered financial math, such as calculating a 15% discount followed by a 20% tax. They guess the answer based on training data. This MCP brings pure, native Javascript logic to percentage math.

### The Superpowers

- **Flawless Financials:** Ensure your AI calculates invoice discounts, VAT taxes, and interest correctly every single time.
- **Absolute Determinism:** No stochastics. Just native mathematical evaluation executed at the edge.


## Available Tools
- **calculate_increase_by**: Increases or decreases a value by X percent deterministically (use negative percent for discount)
- **calculate_percent_of**: Pass the base value and the percentage to compute. Essential for discount calculations, tax rates, and financial reports.

Calculates X percent of a total value deterministically


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Percentage Calculation Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is exactly 15.5% of $2,500.00?"

**🤖 AI Agent:**
> ✅ **Percentage Extracted:** `$387.50`

---

**👤 You:**
> "Add a 20% VAT tax rate to the baseline price of $500."

**🤖 AI Agent:**
> ✅ **Increased Value:** The final price with VAT is `$600.00`.

---

**👤 You:**
> "Apply a 10% coupon discount to the shopping cart total of $1000."

**🤖 AI Agent:**
> ✅ **Decreased Value:** The new cart total is `$900.00`.


## Installation & Usage

To install and use the **Percentage Calculation Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/percentage-calculation-engine](https://vinkius.com/mcp/percentage-calculation-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
