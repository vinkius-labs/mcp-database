# US Pre-judgment Interest Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-pre-judgment-interest-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-pre-judgment-interest-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-pre-judgment-interest-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate statutory pre-judgment interest for US states based on debt amount, default date, and state law.

## Description
This MCP server provides a precise engine to calculate statutory pre-judgment interest across various US jurisdictions. By using tools like `get_state_statute_details`, `calculate_accumulated_interest`, and `list_supported_juris_dictions`, AI agents can determine the legal interest rates (Simple or Compound) for specific states such as California, New York, or Texas. It handles complex date arithmetic to find the exact days elapsed between a default date and a reference date, ensuring compliance with state-specific statutes.


## Available Tools
- **calculate_accumulated_interest**: Calculate total interest accrued on a debt
- **get_state_statute_details**: Get the legal interest rules for a specific state
- **list_supported_jurisdictions**: List all supported US states


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Pre-judgment Interest Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the legal interest rate for California?"

**🤖 AI Agent:**
> The annual statutory interest rate for California is 7%, and it uses the Simple interest calculation method.

---

**👤 You:**
> "Calculate interest for a $10,000 debt in New York that defaulted on 2023-01-01, as of 2024-01-01."

**🤖 AI Agent:**
> $900.00 in total interest has accrued over 365 days.

---

**👤 You:**
> "Which states can I check for interest rates?"

**🤖 AI Agent:**
> The supported jurisdictions include California, New York, and Texas.


## Installation & Usage

To install and use the **US Pre-judgment Interest Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-pre-judgment-interest-calculator](https://vinkius.com/mcp/us-pre-judgment-interest-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
