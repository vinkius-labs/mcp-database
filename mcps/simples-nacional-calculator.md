# Simples Nacional Calculator MCP Server

Calculate effective tax rates, Fator R eligibility, and monthly DAS amounts for the Brazilian Simples Nacional regime.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/simples-nacional-calculator)

## Overview
**Category:** finance
**Tools Count:** 4

## Description
This MCP server provides a precise calculation engine for the Brazilian Simples Nacional taxation system. It allows AI agents to determine complex tax variables by accessing tools like `get_bracket_parameters`, `calculate_effective_rate`, `evaluate_factor_r`, and `compute_monthly_tax_amount`. The server handles progressive revenue tiers across Annexes I through V, calculating the dynamic effective rate based on accumulated revenue (RBT12) and fixed deductions. It also evaluates Fator R eligibility by comparing payroll expenses to gross revenue, enabling accurate estimation of monthly tax liabilities (DAS).


## Available Tools
- **calculate_effective_rate**: Calculate the dynamic effective tax rate
- **compute_monthly_tax_amount**: Calculate the final tax amount due
- **evaluate_factor_r**: Check eligibility for Annex III via Fator R
- **get_bracket_parameters**: Retrieve taxation constants based on activity and revenue


## Installation & Usage

To install and use the **Simples Nacional Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simples-nacional-calculator](https://vinkius.com/mcp/simples-nacional-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
