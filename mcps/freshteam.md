# Freshteam MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshteam)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/freshteam-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/freshteam-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage HR operations, track job applicants, and oversee employee records via AI agents with Freshteam.

## Description
Connect your **Freshteam** account to any AI agent to automate your HR operations and recruitment workflows through the Model Context Protocol (MCP). Freshteam is the smart HR software by Freshworks that handles everything from recruiting and onboarding to time-off management. This MCP server enables you to manage your employee directory, track active job postings, and retrieve applicant data directly through natural conversation.

### Key Features

- **Employee Directory** — List all employees, retrieve detailed HR profiles, and programmatically create new employee records.
- **Recruitment Tracking** — Access your active job postings and list all applicants for specific roles to manage your hiring pipeline.
- **Applicant Discovery** — Retrieve detailed candidate profiles and application statuses instantly.
- **Time-off Management** — Monitor employee time-off requests and leave balances to ensure proper workforce coverage.
- **Organization Structure** — Access configured departments, job roles, and office branches to understand your company's hierarchy.
- **Real-time Synchronization** — Keep your HR data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Freshteam Domain prefix and API Key (found in your Profile Settings)
3. Start managing your HR operations from Claude, Cursor, or any MCP client

### Who is this for?

- **HR Managers** — quickly check employee profiles or time-off requests without manual dashboard navigation.
- **Recruiters** — get a real-time overview of job postings and applicant pipelines via simple AI commands.
- **Department Heads** — monitor team structures and organizational metadata seamlessly.


## Available Tools
- **create_employee_record**: Create an employee
- **check_hris_status**: Verify API connection
- **get_applicant_details**: Get candidate profile
- **get_employee_details**: Get employee metadata
- **get_job_posting_details**: Get job metadata
- **list_job_applicants**: List job candidates
- **list_office_branches**: List office locations
- **list_departments**: List HR departments
- **list_employees**: List HR employees
- **list_job_postings**: List active job openings
- **list_job_roles**: List job roles
- **list_time_off_requests**: List leave requests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshteam** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job postings in Freshteam."

**🤖 AI Agent:**
> Retrieving jobs... I found 3 active job postings, including 'Senior Software Engineer' and 'Marketing Manager'. Would you like to see the applicants for any of these?

---

**👤 You:**
> "Show me the HR profile for employee 'Jane Smith'."

**🤖 AI Agent:**
> Searching employees... I found Jane Smith (jane.smith@example.com). She is a 'Product Manager' in the 'Product' department and is currently 'Active'.

---

**👤 You:**
> "Create a new employee record for 'John Doe' (johndoe@email.com)."

**🤖 AI Agent:**
> Employee created! I have successfully added 'John Doe' (johndoe@email.com) to your HR directory. The new Employee ID is 98765.


## Installation & Usage

To install and use the **Freshteam** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshteam](https://vinkius.com/mcp/freshteam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
