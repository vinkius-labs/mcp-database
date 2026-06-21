# EU Late Payment Interest Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eu-late-payment-interest-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eu-late-payment-interest-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eu-late-payment-interest-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate interest and fixed compensation for overdue commercial payments according to the EU Late/Late Payment Directive (2011/7/EU).

## Description
This MCP server provides a precise way to calculate the financial burden of late B2B payments in the European Union. It automates the complex process of determining interest accrual based on the ECB reference rate plus an 8% margin, as mandated by the EU Late Payment Directive (2011/7/EU). You can use `calculate_accrued_interest` to find the variable cost of delay, `calculate_fixed_compensation` to determine the fixed administrative recovery fee based on debt tiers, or `get_total_overdue_cost` for a comprehensive view of both interest and compensation.


## Available Tools
- **calculate_accrued_interest**: You need the original invoice amount, the due date, and the current calculation date.

Calculates the interest accrued on an unpaid invoice based on the EU Late Payment Directive
- **calculate_fixed_compensation**: The amount depends on the total value of the outstanding debt.

Calculates the fixed administrative recovery fee for an overdue payment
- **get_total_overdue_cost**: Calculates the total financial burden, including both accrued interest and fixed compensation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU Late Payment Interest Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much interest has accumulated on an invoice of €500 that was due on 2024-01-01, calculated as of 2024-06-01?"

**🤖 AI Agent:**
> The interest accrued is €35.89, and the total days overdue is 152 days.

---

**👤 You:**
> "What is the fixed compensation for a debt of €1500?"

**🤖 AI Agent:**
> The fixed administrative recovery fee for an invoice of €1500 is €100.

---

**👤 You:**
> "Calculate the total cost for a €2000 invoice due on 2023-12-01, with calculation date 2024-03-01."

**🤖 AI Agent:**
> The total financial burden is €175.42, consisting of €75.42 in interest and €100.00 in fixed compensation.


## Installation & Usage

To install and use the **EU Late Payment Interest Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eu-late-payment-interest-calculator](https://vinkius.com/mcp/eu-late-payment-interest-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
