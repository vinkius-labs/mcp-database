# Gusto MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gusto)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gusto-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gusto-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage employees, run payroll, view benefits and time-off policies — HR automation for AI agents.

## Description
Connect **Gusto** to any AI agent and streamline your entire HR and payroll operation.

### What you can do

- **Employee Management** — List and view employee profiles with compensation details
- **Payroll Operations** — View payroll runs with earnings, taxes, and deductions
- **Company Info** — Access company details, EIN, and configuration
- **Benefits Administration** — Browse health, dental, 401k, and other benefit plans
- **Time-Off Policies** — View PTO, sick leave, and vacation accrual rates
- **Departments & Locations** — Organizational structure and office locations


## Available Tools
- **list_companies**: List managed companies
- **list_time_off_policies**: List time-off policies
- **get_company**: Get company details
- **list_employees**: List employees in a company
- **get_employee**: Get employee details
- **list_payrolls**: List payroll runs
- **get_payroll**: Get payroll run details
- **list_locations**: List company locations
- **list_departments**: List company departments
- **list_benefits**: ) with enrollment info.

List company benefits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gusto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all employees in the engineering department."

**🤖 AI Agent:**
> Found 12 engineers:

| Name | Title | Start Date |
|------|-------|------------|
| Sarah Chen | Senior Engineer | Jan 2024 |
| Alex Rivera | Staff Engineer | Mar 2023 |
...

---

**👤 You:**
> "Show me the last payroll run details."

**🤖 AI Agent:**
> 📊 Payroll Run — March 31, 2026

| Metric | Value |
|--------|-------|
| Total Gross | $245,000 |
| Federal Tax | -$48,500 |
| State Tax | -$12,200 |
| Net Pay | $184,300 |
| Employees | 34 |

---

**👤 You:**
> "List all time-off policies."

**🤖 AI Agent:**
> 3 policies configured:

1. **Unlimited PTO** — Salaried employees
2. **Sick Leave** — 10 days/year, accrual-based
3. **Parental Leave** — 12 weeks paid


## Installation & Usage

To install and use the **Gusto** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gusto](https://vinkius.com/mcp/gusto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
