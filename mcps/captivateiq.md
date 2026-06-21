# CaptivateIQ MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/captivateiq)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/captivateiq-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/captivateiq-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage incentive compensation via CaptivateIQ — track commission payouts, statements, and employee plans directly from any AI agent.

## Description
Connect your **CaptivateIQ** account to any AI agent and orchestrate your incentive compensation, commission tracking, and payroll integration workflows through natural conversation.

### What you can do

- **Payout Oversight** — List and retrieve detailed metadata for all processed commission payouts across your organization.
- **Statement Management** — Access individualized payout statements for employees to verify earnings and calculations.
- **Employee Coordination** — List and retrieve detailed profiles for all employees, including their plan designations and hierarchy.
- **Workbook Monitoring** — Access and list your calculation workbooks and worksheets to ensure transparency in your commission logic.
- **Dispute Tracking** — Monitor and list commission inquiries or disputes directly from your workspace.
- **Financial Reporting** — Retrieve core account and integration information straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your CaptivateIQ API Token
3. Start managing your commission data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance & Payroll Teams** — quickly extract payout data for payroll runs without manual dashboard exports.
- **Sales Operations** — monitor commission trends and employee designations straight from their workflow tools.
- **Revenue Leaders** — retrieve high-level payout summaries and plan details using natural language.


## Available Tools
- **get_account_status**: Retrieve core account/integration information
- **get_employee_details**: Get details of a specific employee
- **list_employees**: List all employee records and plan designations
- **list_commission_inquiries**: List commission disputes and inquiries (generic search)
- **list_commission_payouts**: List all processed commission payouts
- **list_payout_statements**: List individualized payout statements for employees
- **list_workbooks**: List all calculation workbooks
- **list_worksheets**: List all calculation worksheets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CaptivateIQ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all processed commission payouts in CaptivateIQ."

**🤖 AI Agent:**
> I've retrieved your payouts. You have several recent payouts, including 'March Sales Cycle' (Total: $120,000) and 'Q1 Bonus Run' (Total: $45,000).

---

**👤 You:**
> "Show the payout statement for employee John Doe."

**🤖 AI Agent:**
> Retrieving statement for John Doe... For the last period, he earned a total commission of $4,500 based on his sales target attainment of 110%.

---

**👤 You:**
> "Which calculation workbooks are available in my account?"

**🤖 AI Agent:**
> You have 3 active workbooks: 'Global Sales Plan 2026', 'Manager Incentive Tier', and 'Referral Program Logic'. Which one would you like to explore?


## Installation & Usage

To install and use the **CaptivateIQ** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/captivateiq](https://vinkius.com/mcp/captivateiq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
