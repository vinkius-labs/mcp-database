# SAP Concur MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sap-concur)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sap-concur-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sap-concur-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Enable your AI agent to manage corporate expenses, track report statuses, and retrieve user profiles via the SAP Concur API.

## Description
Connect your AI assistant to **SAP Concur**, the leading platform for expense management, travel, and invoice automation.

### What you can do

- **Expense Tracking** — List and inspect individual expenses including amounts, categories, and receipt metadata.
- **Report Status** — Check approval status of any expense report.
- **User Profiles** — Retrieve employee profile data including cost center and department.

### How it works

1. Add the SAP Concur integration.
2. Register an app in the SAP Concur Developer Portal and provide the Client ID, Client Secret, and Refresh Token.
3. Query expense data via natural language commands.

### Who is this for?

- **Finance Teams** — Pull expense summaries without logging into the dashboard.
- **Travel Managers** — Verify travel policy compliance in real time.
- **Employees** — Check approval status of their own reports from chat.


## Available Tools
- **get_expense**: Retrieve detailed information about a specific expense
- **list_pending_expenses**: Quickly list all expenses that have not yet been assigned to a report
- **get_expense_report**: Retrieve detailed information about a specific expense report
- **get_report_summaries**: Calculate basic totals for a list of recent expense reports
- **get_user_profile**: Retrieve the profile details of the currently authenticated Concur user
- **list_attendees**: Retrieve a list of expense attendees (for business meals, etc.)
- **list_expense_types**: Retrieve a list of valid expense types configured in your organization
- **list_expenses**: Retrieve a list of your expenses from Concur
- **list_expense_reports**: Retrieve a list of your expense reports from Concur


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SAP Concur** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my last 10 expenses in Concur."

**🤖 AI Agent:**
> Here are your 10 most recent expenses:
1. Uber ride — $24.50 (Jan 22)
2. Hotel — $189.00 (Jan 20)
3. Lunch meeting — $47.80 (Jan 18)
Would you like the full report for any of these?

---

**👤 You:**
> "Get the status of expense report 'rep-8842'."

**🤖 AI Agent:**
> Report 'rep-8842' is **Pending Approval**. Submitted by John Smith on Jan 20 with 5 entries totaling $412.30. Approver: Sarah Wilson.

---

**👤 You:**
> "Retrieve the profile for employee 'E-4545'."

**🤖 AI Agent:**
> Employee Profile:
- Name: Michael Davis
- ID: E-4545
- Department: Sales
- Cost Center: NA-West (CC-102)
- Manager ID: E-3300


## Installation & Usage

To install and use the **SAP Concur** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sap-concur](https://vinkius.com/mcp/sap-concur)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
