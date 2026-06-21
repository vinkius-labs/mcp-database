# EU Limitation Periods Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eu-limitation-periods-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eu-limitation-periods-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eu-limitation-periods-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate statutory limitation periods and expiry dates for European jurisdictions.

## Description
This MCP server provides a precise way to determine the statutes of limitations across various European legal systems. Using tools like `get_limitation_info`, you can retrieve the standard duration, starting point logic, and interruption causes for specific countries such as Germany (DE), France (FR), Spain (ES), and Portugal (PT). Additionally, the `calculate_expiry_date` tool allows you to input an event date to find the exact calendar day when a legal claim expires. It is designed to bridge AI agents with complex jurisdictional data, ensuring accurate tracking of legal deadlines.


## Available Tools
- **get_limitation_info**: Evaluates the standard duration, starting point logic, and interruption causes for a specific country and relationship type
- **list_supported_jurisdictions**: Provides a list of all European countries currently serviced by the calculator
- **calculate_expiry_date**: Determines the exact calendar date when a claim will expire based on a known starting event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU Limitation Periods Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the limitation period for a contractual obligation in Germany?"

**🤖 AI Agent:**
> The standard limitation period for contractual obligations in Germany (DE) is 3 years.

---

**👤 You:**
> "Calculate when a claim starting on 2023-01-01 in Spain will expire."

**🤖 AI Agent:**
> For a delictual obligation in Spain (ES) starting on 2023-01-01, the claim will expire on 2028-01-01.

---

**👤 You:**
> "List all supported jurisdictions."

**🤖 AI Agent:**
> The supported jurisdictions are: DE, FR, ES, PT.


## Installation & Usage

To install and use the **EU Limitation Periods Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eu-limitation-periods-calculator](https://vinkius.com/mcp/eu-limitation-periods-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
