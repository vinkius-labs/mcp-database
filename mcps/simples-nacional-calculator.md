# Simples Nacional Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simples-nacional-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/simples-nacional-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/simples-nacional-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate effective tax rates, Fator R eligibility, and monthly DAS amounts for the Brazilian Simples Nacional regime.

## Description
This MCP server provides a precise calculation engine for the Brazilian Simples Nacional taxation system. It allows AI agents to determine complex tax variables by accessing tools like `get_bracket_parameters`, `calculate_effective_rate`, `evaluate_factor_r`, and `compute_monthly_tax_amount`. The server handles progressive revenue tiers across Annexes I through V, calculating the dynamic effective rate based on accumulated revenue (RBT12) and fixed deductions. It also evaluates Fator R eligibility by comparing payroll expenses to gross revenue, enabling accurate estimation of monthly tax liabilities (DAS).


## Available Tools
- **calculate_effective_rate**: Calculate the dynamic effective tax rate
- **compute_monthly_tax_amount**: Calculate the final tax amount due
- **evaluate_factor_r**: Check eligibility for Annex III via Fator R
- **get_bracket_parameters**: Retrieve taxation constants based on activity and revenue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Simples Nacional Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the effective tax rate for a company with 200,000 BRL accumulated revenue in Annex I, using a nominal rate of 4% and deduction of 0."

**🤖 AI Agent:**
> The effective tax rate is 4.0%.

---

**👤 You:**
> "Check if a company with 100,000 BRL revenue and 30,000 BRL payroll qualifies for Fator R."

**🤖 AI Agent:**
> The company is eligible for the lower taxation tier (Annex III) because the payroll-to-revenue ratio is 30%.

---

**👤 You:**
> "How much tax will I pay this month if my revenue is 5,000 BRL and my effective rate is 6%?"

**🤖 AI Agent:**
> The total tax due (DAS) for this month is 300.00 BRL.


## Installation & Usage

To install and use the **Simples Nacional Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simples-nacional-calculator](https://vinkius.com/mcp/simples-nacional-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
