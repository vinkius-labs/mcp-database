# ISS Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iss-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/iss-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/iss-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Service Tax (ISS) based on municipality rates and service types.

## Description
This MCP server provides specialized tools for calculating Service Tax (ISS). Use `get_applicable_rate` to find the tax percentage for a specific municipality and service type, `check_withholding_status` to determine if tax must be withheld at source, and `calculate_tax_liability` to compute the final taxable base and tax amount including any allowed deductions.


## Available Tools
- **calculate_tax_liability**: Calculate final tax liability
- **check_withholding_status**: Check if tax withholding is required
- **get_applicable_rate**: Get the tax rate for a service in a municipality


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ISS Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the tax rate for IT services in Sao Paulo?"

**🤖 AI Agent:**
> To find this, you should call `get_applicable_rate` with municipalityName: 'Sao Paulo' and serviceType: 'IT Services'.

---

**👤 You:**
> "Calculate the tax for a 1000 gross amount cleaning service in Rio de Janeiro with 200 deduction."

**🤖 AI Agent:**
> You can use `calculate_tax_liability` with municipalityName: 'Rio de Janeiro', serviceType: 'Cleaning', grossAmount: 1000, and deductionAmount: 200.

---

**👤 You:**
> "Is withholding required for construction services in Belo Horizonte?"

**🤖 AI Agent:**
> Use the `check_withholding_status` tool with municipalityName: 'Belo Horizonte' and serviceType: 'Construction' to verify this.


## Installation & Usage

To install and use the **ISS Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iss-calculator](https://vinkius.com/mcp/iss-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
