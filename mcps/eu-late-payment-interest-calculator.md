# EU Late Payment Interest Calculator MCP Server

Calculate interest and fixed compensation for overdue commercial payments according to the EU Late/Late Payment Directive (2011/7/EU).

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/eu-late-payment-interest-calculator)

## Overview
**Category:** finance
**Tools Count:** 3

## Description
This MCP server provides a precise way to calculate the financial burden of late B2B payments in the European Union. It automates the complex process of determining interest accrual based on the ECB reference rate plus an 8% margin, as mandated by the EU Late Payment Directive (2011/7/EU). You can use `calculate_accrued_interest` to find the variable cost of delay, `calculate_fixed_compensation` to determine the fixed administrative recovery fee based on debt tiers, or `get_total_overdue_cost` for a comprehensive view of both interest and compensation.


## Available Tools
- **calculate_accrued_interest**: You need the original invoice amount, the due date, and the current calculation date.

Calculates the interest accrued on an unpaid invoice based on the EU Late Payment Directive
- **calculate_fixed_compensation**: The amount depends on the total value of the outstanding debt.

Calculates the fixed administrative recovery fee for an overdue payment
- **get_total_overdue_cost**: Calculates the total financial burden, including both accrued interest and fixed compensation


## Installation & Usage

To install and use the **EU Late Payment Interest Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eu-late-payment-interest-calculator](https://vinkius.com/mcp/eu-late-payment-interest-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
