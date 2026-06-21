# Days Between Dates Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/days-between-dates-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/days-between-dates-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/days-between-dates-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise intervals between two dates in years, months, weeks, and days.

## Description
This MCP server provides specialized tools to calculate the exact time elapsed between two dates. Use `get_date_breakdown` to receive a detailed breakdown of years, months, weeks, and days. You can also use `count_business_days` to determine the number of working days between two periods while optionally excluding regional holidays in the USA or Europe. Additionally, `verify_holiday_status` allows you to check if a specific date is recognized as a national holiday within your selected region.


## Available Tools
- **count_business_days**: Calculates the total number of working days between two dates
- **get_date_breakdown**: Provides a detailed breakdown of the time elapsed between two dates
- **verify_holiday_status**: Checks if a specific date is recognized as a national holiday in a given region


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Days Between Dates Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days are between 2023-01-01 and 2023-12-31?"

**🤖 AI Agent:**
> You can use `get_date_breakdown` with startDate: '2023-01-01' and endDate: '2023-12-31' to see the exact breakdown.

---

**👤 You:**
> "Check if 2024-07-04 is a holiday in the USA."

**🤖 AI Agent:**
> The `verify_holiday_status` tool can confirm this by checking targetDate: '2024-07-04' and region: 'USA'.

---

**👤 You:**
> "Calculate working days between 2024-01-01 and 2024-01-10, excluding holidays."

**🤖 AI Agent:**
> Use `count_business_days` with startDate: '2024-01-01', endDate: '2024-01-10', and excludeHolidays: true.


## Installation & Usage

To install and use the **Days Between Dates Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/days-between-dates-calculator](https://vinkius.com/mcp/days-between-dates-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
