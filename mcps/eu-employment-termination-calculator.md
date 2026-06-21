# EU Employment Termination Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eu-employment-termination-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eu-employment-termination-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eu-employment-termination-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate statutory severance pay for Germany, France, Spain, and Portugal.

## Description
This MCP server provides precise calculations for statutory employment termination compensation across key European jurisdictions. Using the `calculate_severance` tool, you can estimate severance amounts based on monthly salary, years of service, and dismissal type for Germany (DE), France (FR), Spain (ES), and Portugal (PT). The server also includes `get_country_policy` to retrieve specific legal formulas and `validate_eligibility` to check if a termination event qualifies for statutory pay.


## Available Tools
- **calculate_severance**: Calculates the estimated monetary compensation for an employee termination
- **get_country_policy_summary**: g., France 10-year cap).

Retrie ives the legal rules used for a specific country's calculations
- **validate_termination_eligibility**: Checks whether a specific dismissal type is legally eligible to trigger compensation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU Employment Termination Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate severance for a German employee with 5 years of service and 3000 EUR monthly salary."

**🤖 AI Agent:**
> The `calculate_severance` tool would return an estimated amount based on half a monthly salary for each year of service.

---

**👤 You:**
> "What is the legal policy for France?"

**🤖 AI Agent:**
> Using `get_country_policy` for FR, you would see the rule regarding one quarter of a monthly salary per year up to 10 years.

---

**👤 You:**
> "Is a dismissal in Spain eligible for compensation?"

**🤖 AI Agent:**
> The `validate_eligibility` tool would check the dismissal type against Spanish labor laws.


## Installation & Usage

To install and use the **EU Employment Termination Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eu-employment-termination-calculator](https://vinkius.com/mcp/eu-employment-termination-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
