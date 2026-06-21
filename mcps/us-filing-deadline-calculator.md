# US Filing Deadline Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-filing-deadline-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-filing-deadline-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-filing-deadline-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate US federal court filing deadlines with automatic weekend and holiday adjustments.

## Description
This MCP server provides specialized tools for legal professionals to determine US federal procedural filing deadlines. By using `calculate_deadline`, you can input an event date and a rule type (such as RULE_12 or NOTICE_OF_APPEAL) to find the final deadline, automatically adjusted for weekends and federal holidays. The server also includes `list_supported_rules` to browse available legal rules and `check_date_validity` to verify if a specific date is a valid business day for starting a legal clock.


## Available Tools
- **calculate_deadline**: Determines the final filing deadline for a specific event and rule type
- **check_date_validity**: Validates whether a provided date is a viable starting point for a legal clock
- **list_supported_rules**: Provides a list of all legal rules currently supported by the calculator


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Filing Deadline Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the deadline for an event that occurred on 2024-01-01 using RULE_12."

**🤖 AI Agent:**
> The final filing deadline is 2024-01-23.

---

**👤 You:**
> "What are the supported rules?"

**🤖 AI Agent:**
> The available rules are: RULE_12, NOTICE_OF_APPEAL, and RULE_59.

---

**👤 You:**
> "Is 2024-07-04 a valid business day?"

**🤖 AI Agent:**
> No, 2024-07-04 is a holiday (Independence Day).


## Installation & Usage

To install and use the **US Filing Deadline Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-filing-deadline-calculator](https://vinkius.com/mcp/us-filing-deadline-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
