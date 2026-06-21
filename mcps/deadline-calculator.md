# Deadline Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deadline-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/deadline-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/deadline-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise end dates by adding calendar or business days, accounting for weekends and regional holidays.

## Description
The Deadline Calculator MCP server provides specialized tools to determine exact completion dates. Use `calendar_deadline_tool` to calculate end dates by adding uninterrupted calendar days, or use `business_deadline_tool` to compute deadlines that skip weekends and regional holidays in the US, UK, Germany, or France. You can also use `holiday_registry_tool` to retrieve a list of recognized holidays for a specific region and year to verify your calculations.


## Available Tools
- **business_deadline_tool**: Calculate a deadline by adding business days to a start date
- **calendar_deadline_tool**: Calculate a deadline by adding calendar days to a start date
- **holiday_registry_tool**: Fetch the holiday registry for a specific region and year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deadline Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the end date if I start on 2024-01-01 and add 10 calendar days."

**🤖 AI Agent:**
> Using `calendar_deadline_tool`, the calculated end date is 2024-01-11.

---

**👤 You:**
> "What is the deadline for a 5 business day task starting on 2024-07-01 in the US?"

**🤖 AI Agent:**
> The `business_deadline_tool` calculates the end date as 2024-07-08, accounting for the July 4th holiday in the US.

---

**👤 You:**
> "List all holidays in Germany for the year 2024."

**🤖 AI Agent:**
> The `holiday_registry_tool` returns a list of all registered German holidays for 2024, including New Year's Day and German Unity Day.


## Installation & Usage

To install and use the **Deadline Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deadline-calculator](https://vinkius.com/mcp/deadline-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
