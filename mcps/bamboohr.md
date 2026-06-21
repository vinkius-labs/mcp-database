# BambooHR MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bamboohr)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bamboohr-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bamboohr-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Official HR software automation — manage employee directories, time off requests, and company reports via AI.

## Description
Orchestrate your human resources operations with **BambooHR**, the leading platform for small and medium businesses. By connecting BambooHR to your AI agent, you transform complex people management into a natural conversation. Your agent can instantly search the employee directory, audit time off requests, identify who is out of the office today, and retrieve custom company reports without you ever navigating through dense HR menus. Whether you're a manager checking team availability or an HR admin updating records, your agent acts as a direct bridge to your people data, ensuring your organizational culture stays agile and informed.

### What you can do

- **Employee Directory** — Search and list active employees, retrieving basic contact details and profile information through natural language.
- **Time Off Management** — Audit active time off requests, list employees currently out of the office, and submit new requests seamlessly.
- **HR Auditing** — Retrieve specific company reports and list available time off types or policies for your organization.
- **Record Updates** — Programmatically update basic employee information to ensure your HR records are always accurate.
- **Availability Insights** — Quickly identify team members who are out for specific date ranges to optimize project planning.

### How it works

1. Subscribe to this server
2. Enter your BambooHR Subdomain and API Key
3. Start managing your human resources through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Team Managers** — check who is out of the office today and audit time off requests for your team directly from chat.
- **HR Administrators** — retrieve company reports and update employee records without manual dashboard entry.
- **Operations Leads** — verify employee contact details and organizational structures for project coordination.
- **Knowledge Workers** — quickly find teammates' information and availability through natural conversation.


## Available Tools
- **add_time_off_request**: Submit a new time off request for an employee
- **get_account_check**: Verify BambooHR connection
- **get_company_report**: Get a specific company report by ID
- **get_employee_details**: Get basic details for a specific employee
- **list_employees_directory**: List active employees from the company directory
- **list_time_off_policies**: List all defined time off policies
- **list_time_off_requests**: List time off requests
- **list_time_off_types**: List all defined time off types
- **list_whos_out**: Helper to list who is out today
- **search_employee**: Search for an employee by name in the directory
- **update_employee**: Update employee information
- **whos_out**: List employees who are out (time off) for a date range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BambooHR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who is out of the office today?"

**🤖 AI Agent:**
> Checking BambooHR... Today, Jane Doe (Vacation) and John Smith (Sick Leave) are out. Would you like to check availability for a different date range?

---

**👤 You:**
> "Search for 'Sarah' in the employee directory."

**🤖 AI Agent:**
> I found Sarah Miller. She is a 'Senior Engineer' in the 'Product' team. Her email is sarah.miller@example.com. Would you like her extension or office location?

---

**👤 You:**
> "What are my available time off types?"

**🤖 AI Agent:**
> Retrieving time off types... You have access to: Vacation, Sick Leave, Personal Day, and Bereavement. Which one would you like to request?


## Installation & Usage

To install and use the **BambooHR** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bamboohr](https://vinkius.com/mcp/bamboohr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
