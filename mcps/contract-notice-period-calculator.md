# Contract Notice Period Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contract-notice-period-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/contract-notice-period-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/contract-notice-period-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal](../categories/legal.md)

Calculate minimum legal notice periods and effective termination dates for various contract types across USA and Europe.

## Description
This MCP server provides a precise engine to determine the mandatory minimum notice periods and calculate exact termination dates. By using tools like `get_notice_requirement`, you can retrieve legal requirements for employment, commercial leases, and service agreements across specific US states and European nations. Additionally, use `calculate_effective_date` to find the final day of a contract based on your notice date, or `check_jurisdiction_validity` to verify if a region is within the supported regulatory scope.


## Available Tools
- **get_notice_requirement**: Retrieves the mandatory minimum notice period and its associated legal description
- **calculate_effective_date**: Determines the exact date a contract will end
- **check_jurisdiction_validity**: Validates if a provided location is within the supported legal scope


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contract Notice Period Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum notice period for an employment contract in California?"

**🤖 AI Agent:**
> The `get_notice_requirement` tool would be used to retrieve the specific days and legal description for California.

---

**👤 You:**
> "Calculate the end date if I gave notice on 2024-01-01 with a 30 day period."

**🤖 AI Agent:**
> The `calculate_effective_date` tool will return the calculated termination date based on those inputs.

---

**👤 You:**
> "Is Germany a supported jurisdiction?"

**🤖 AI Agent:**
> You can use `check_jurisdiction_validity` to confirm if Germany is within the supported scope and see its regulatory level.


## Installation & Usage

To install and use the **Contract Notice Period Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contract-notice-period-calculator](https://vinkius.com/mcp/contract-notice-period-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
