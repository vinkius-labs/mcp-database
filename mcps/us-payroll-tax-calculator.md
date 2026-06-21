# US Payroll Tax Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-payroll-tax-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-payroll-tax-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-payroll-tax-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise US payroll tax liabilities, including FICA, Medicare, FUTA, and SUTA.

## Description
This MCP server provides tools to calculate various United States payroll tax obligations. Use `calculate_employee_withholdings` to determine employee-side deductions like Social Security and Medicare. Use `calculate_employer_liabilities` to find employer costs including FUTA and state-specific SUTA based on the provided state code. Finally, use `get_payroll_summary` for a high-level comparison of net pay versus total company cost.


## Available Tools
- **calculate_employee_withholdings**: Calculate employee-side tax withholdings
- **calculate_employer_liabilities**: Calculate employer-side tax liabilities
- **get_payroll_summary**: Get a high-level payroll summary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Payroll Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate how much will be withheld from an employee earning $75,000 per year."

**🤖 AI Agent:**
> The `calculate_employee_withholdings` tool will return the Social Security, Medicare, and any additional Medicare withholdings for a $75,000 salary.

---

**👤 You:**
> "What are the employer tax liabilities for an employee in California earning $100,000?"

**🤖 AI Agent:**
> Using `calculate_employer_liabilities` with annualGrossPay: 100000 and stateCode: 'CA' will provide the Social Security, Medicare, FUTA, and SUTA liabilities.

---

**👤 You:**
> "Provide a payroll summary for $150,000 gross pay in Texas."

**🤖 AI Agent:**
> The `get_payroll_summary` tool will calculate the net employee pay, total employer cost, and the aggregate tax burden for $150,000 in TX.


## Installation & Usage

To install and use the **US Payroll Tax Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-payroll-tax-calculator](https://vinkius.com/mcp/us-payroll-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
