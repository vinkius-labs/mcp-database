# Scholarship Eligibility Checker MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scholarship-eligibility-checker)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/scholarship-eligibility-checker-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/scholarship-eligibility-checker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate household per capita income and determine eligibility for scholarship programs like ProUni and FIES.

## Description
This MCP server provides tools to calculate household per capita income and check eligibility for various scholarship programs. Use `calculate_per_capita_income` to compute the economic share of a household, `check_program_eligibility` to verify if a student qualifies for specific grants based on income thresholds, and `retrieve_program_requirements` to fetch detailed rules and multipliers for programs like PROUNI or FIES.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scholarship Eligibility Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate per capita income for 5000 gross income and 4 members."

**🤖 AI Agent:**
> The calculated per capita income is 1250.

---

**👤 You:**
> "Am I eligible for PROUNI_FULL with 1000 per capita income?"

**🤖 AI Agent:**
> Yes, you are eligible for PROUNI_FULL with 100% coverage.

---

**👤 You:**
> "What are the rules for STATE_GRANT?"

**🤖 AI Agent:**
> The `retrieve_program_requirements` tool shows that STATE_GRANT allows up to 2x the minimum wage.


## Installation & Usage

To install and use the **Scholarship Eligibility Checker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scholarship-eligibility-checker](https://vinkius.com/mcp/scholarship-eligibility-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
