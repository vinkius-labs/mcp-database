# Holiday API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/holiday-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/holiday-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/holiday-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage global holidays — audit public and federal holidays via AI.

## Description
Empower your AI agent to orchestrate your entire global event and holiday research workflow with **Holiday API**, the reliable source for holiday data. By connecting Holiday API to your agent, you transform complex calendar auditing into a natural conversation. Your agent can instantly retrieve public holidays for any country, audit workday counts, and identify supported languages without you ever touching a manual calendar. Whether you are planning international logistics or managing global payroll, your agent acts as a real-time event consultant, ensuring your schedules are always accurate and compliant.

### What you can do

- **Holiday Auditing** — Retrieve public and federal holidays for over 200 countries and retrieve detailed metadata, including names and dates.
- **Workday Oversight** — Calculate the next workday or count workdays between two dates to maintain a clear view of operational periods.
- **Global Discovery** — List all supported countries and languages in the Holiday API catalog to identify regional event markers.
- **Temporal Intelligence** — Query holidays for specific years to audit past and future global events instantly.
- **Usage Monitoring** — Get real-time API usage and status metadata to maintain strict control over your research volume.

### How it works

1. Subscribe to this server
2. Enter your Holiday API Key
3. Start managing your event intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Managers** — monitor international holidays and retrieve workday metadata straight from your workflow.
- **HR Specialists** — verify global public holidays and audit payroll cycles without manual searching.
- **Travel Planners** — perform rapid audits of local events and identify peak holiday periods through natural language.
- **Operations Leads** — automate holiday data querying to orchestrate cross-functional global teams smoothly.


## Available Tools
- **get_holidays**: Get public holidays for a country and year
- **get_next_workday**: Get the date after a number of workdays from a start date
- **get_workdays_count**: Count the number of workdays between two dates
- **list_supported_countries**: List all countries supported by Holiday API
- **list_supported_languages**: List all languages supported by Holiday API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Holiday API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the public holidays in 'US' for 2024 using Holiday API?"

**🤖 AI Agent:**
> I've retrieved the 2024 public holidays for the United States. Notable dates include Independence Day on July 4th and Thanksgiving on November 28th. Would you like the full list of federal holidays?

---

**👤 You:**
> "Calculate the next 10 workdays from 2024-01-01 in Brazil."

**🤖 AI Agent:**
> I've calculated the date! After 10 workdays in Brazil starting from January 1st, 2024, the resulting date is January 15th, 2024. I've accounted for the New Year's holiday.

---

**👤 You:**
> "List all countries supported by Holiday API."

**🤖 AI Agent:**
> I've scanned the country catalog. Holiday API supports over 200 countries, including United Kingdom, Germany, and Japan. I can provide the country codes for any of them.


## Installation & Usage

To install and use the **Holiday API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/holiday-api](https://vinkius.com/mcp/holiday-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
