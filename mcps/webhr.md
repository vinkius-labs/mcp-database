# WebHR MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webhr)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/webhr-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/webhr-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage employees, attendance, and recruitment on WebHR with AI agents.

## Description
Connect your **WebHR** account to any AI agent to automate your human resource management and personnel tracking. WebHR provides a comprehensive cloud-based HRMS for managing the entire employee lifecycle—from recruitment and onboarding to attendance monitoring and leave management.

### What you can do

- **Employee Orchestration** — List and retrieve detailed metadata for all staff records, including personal profiles and department hierarchies.
- **Attendance Monitoring** — Access real-time clock-in/out records and retrieve aggregated attendance summaries for your organization.
- **Leave Management** — Track leave requests, monitor balance details, and list different leave types available in your system.
- **Recruitment Control** — Monitor open job postings, list active candidates, and manage the recruitment pipeline programmatically.
- **Structural Oversight** — Access company locations and department definitions to maintain a clear overview of your organizational structure.

### How it works

1. Subscribe to this server
2. Enter your WebHR API Key from your Setup settings
3. Start managing your human resources from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — automate the monitoring of staff attendance and recruitment progress via natural language.
- **Operations Leads** — quickly retrieve employee details and department structures without switching applications.
- **Business Owners** — get instant summaries of organizational health and personnel metrics straight through the chat.


## Available Tools
- **get_attendance_summary**: Get aggregated attendance metrics
- **get_employee_details**: Get details for an employee
- **list_attendance_logs**: List clock-in/out records
- **list_job_candidates**: List applicants for positions
- **list_company_departments**: g. Sales, Engineering).

List organizational departments
- **list_employees**: List organization employees
- **list_job_postings**: List open job positions
- **list_job_requests**: List internal job requisitions
- **list_available_leave_types**: List categories of leave
- **list_leave_requests**: List employee leave history
- **list_office_locations**: List company offices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WebHR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of our open 'Senior Frontend Engineer' job posting and list all the active candidates currently in the pipeline."

**🤖 AI Agent:**
> The 'Senior Frontend Engineer' position is currently active. I found 8 active candidates in the pipeline, with 3 in the 'Technical Interview' stage and 5 in 'Screening'. Would you like to view the details of any specific candidate?

---

**👤 You:**
> "Retrieve all pending leave requests for the Engineering department and check the available vacation balance for 'Marcus Johnson'."

**🤖 AI Agent:**
> There are currently 4 pending leave requests in the Engineering department. I also checked Marcus Johnson's profile: his request for 5 days of PTO is pending, and he currently has 12 days of vacation balance remaining.

---

**👤 You:**
> "Generate an attendance summary for the New York office to see how many employees clocked in late this week."

**🤖 AI Agent:**
> I've pulled the attendance summary for the New York office. This week, there were 145 successful on-time clock-ins and 12 late arrivals. The overall punctuality rate is currently at 92%. Would you like a detailed log of the late entries?


## Installation & Usage

To install and use the **WebHR** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webhr](https://vinkius.com/mcp/webhr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
