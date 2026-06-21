# Remote MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/remote)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/remote-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/remote-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Hire and pay global employees and contractors with compliant payroll, benefits, and employment infrastructure across 60+ countries.

## Description
Connect your **Remote** account to any AI agent to streamline your global hiring, payroll, and compliance workflows. Remote provides a powerful RESTful platform for programmatically managing international teams, tracking employee data, and monitoring invoices across 150+ countries.

### What you can do

- **Company Orchestration** — List and retrieve detailed metadata for all your registered company entities and their operational status.
- **Global Talent Management** — Access and monitor your global workforce, track employee profile data, and create new employee records programmatically.
- **International Compliance Monitoring** — List all countries supported by Remote to understand your global hiring capacity and requirements.
- **Invoice & Financial Tracking** — Access and monitor company invoices to ensure transparent and timely global payroll operations.
- **HR Intelligence** — Get a real-time overview of your international workforce and hiring trends using natural language commands.

### How it works

1. Subscribe to this server
2. Enter your Remote API Key from your developer settings at remote.com
3. Start managing your global HR from Claude, Cursor, or any MCP client

### Who is this for?

- **Global HR & Finance Teams** — monitor international payroll and employee data using natural language.
- **Operations Managers** — automate the onboarding of new global hires and track invoice statuses more efficiently.
- **Developers** — integrate real-time HR and compliance data into custom business dashboards.


## Available Tools
- **create_employee**: Pass data as a JSON string.

Add a new employee
- **get_company_details**: Get specific company details
- **get_employee**: Get details for a specific employee
- **get_invoice_details**: Get details for a specific invoice
- **list_companies**: List all registered companies
- **list_contractors**: List all contractors
- **list_supported_countries**: List all countries supported by Remote
- **list_employees**: List employees for a company
- **list_expenses**: List all employee expenses
- **list_invoices**: List invoices for a company
- **list_timeoff**: List all time-off requests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Remote** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active companies in my Remote account."

**🤖 AI Agent:**
> I've retrieved your companies. You have 3 active entities, including 'Vinkius Global' and 'Tech Pilots LLC'. Which one would you like to see employees for?

---

**👤 You:**
> "Show me all employees across all countries with their contract types and compensation details."

**🤖 AI Agent:**
> 47 employees across 12 countries. By region: Americas (18), Europe (16), APAC (13). Contract types: Full-time (38), Part-time (5), Contractor (4). Top countries: US (12), UK (8), Germany (6), Brazil (5), India (4). Average salary: $85,200. Total monthly payroll: $334,000. 3 employees have pending onboarding in Portugal, Japan, and Canada. 2 contract renewals due this month. Benefits utilization: health insurance 94%, equipment allowance 78%.

---

**👤 You:**
> "List all pending time-off requests that need manager approval this week."

**🤖 AI Agent:**
> 8 pending time-off requests. Sarah Chen (Germany): 5 days vacation Jun 2-6, 18 days remaining. James Park (US): 3 days personal May 26-28. Lisa Wang (Brazil): 2 days sick leave May 19-20. Alex Rivera (UK): 10 days vacation Jun 16-27 (team coverage confirmed). 4 additional requests from India (2), Canada (1), Japan (1). No conflicts detected with current project deadlines. 2 requests overlap with the sprint planning week, flagged for review.


## Installation & Usage

To install and use the **Remote** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/remote](https://vinkius.com/mcp/remote)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
