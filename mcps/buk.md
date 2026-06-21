# Buk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/buk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/buk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate your HR and Payroll data via Buk — query employees, list vacations, extract company charts, and orchestrate talent operations directly from any AI agent.

## Description
Connect your **Buk** organizational environment to any AI agent and oversee your Latin American HR operations seamlessly through natural conversation.

### What you can do

- **Talent Discovery** — Query your entire employee database, extracting current operational roles, internal IDs, and hierarchical positions.
- **Absence & Vacations** — Read the historic and upcoming scheduled time loops (vacations/leaves) to perfectly orchestrate team capacity via the bot.
- **Organizational Architecture** — Extract detailed internal departments (Cost Centers) and cross-reference them to build structural overviews.
- **Job Catalogs** — Verify the registered taxonomy of job positions available inside your corporative setup.

### How it works

1. Subscribe to this server
2. Enter your Buk API Key & Company Domain
3. Gain complete analytical power to inspect your HR data inside Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **HR Directors & Managers** — Swiftly analyze department sizes or who is on vacation without authenticating inside the web portals.
- **Operations Leads** — Retrieve specific IDs and talent availability dynamically to feed workflow planning structures.
- **SysAdmins & Tech Teams** — Debug and cross-reference active internal employees instantly against engineering datasets.


## Available Tools
- **get_company_stats**: Get company HR aggregate stats
- **get_department**: Get department details
- **get_employee**: Get complete details of a specific talent
- **list_departments**: List all organizational departments (cost centers)
- **list_employees**: List all employees inside the Buk platform
- **list_jobs**: List standard job roles
- **list_leaves**: List absence leaves
- **list_vacations**: List scheduled vacations
- **approve_leave**: Authorize pending leaves
- **create_employee**: Onboard a new employee to system
- **delete_employee**: Offboard an employee identity
- **get_attendance**: Fetch daily attendance matrix
- **get_payroll**: Get employee payroll snapshot
- **list_benefits**: View available corporate extras


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the organizational structure and show me our standard list of Departments."

**🤖 AI Agent:**
> Departments retrieved! You currently have 'Engineering' (ID: 102), 'Commercial & Sales' (ID: 104), and 'HR Ops' (ID: 105). Do you need me to query employees inside Engineering?

---

**👤 You:**
> "Can you check the current scheduled vacations for the employee named Fernando Silva?"

**🤖 AI Agent:**
> Searching... Fernando Silva (ID: 9812) has a pending vacation schedule approved. He will be out from March 12th to March 25th (13 days). No other leaves detected.

---

**👤 You:**
> "Pull a high priority company overview from our Buk metrics."

**🤖 AI Agent:**
> The overview shows you currently support 143 active employees traversing across 15 formalized departments. Your corporate footprint indicates solid scaling numbers.


## Installation & Usage

To install and use the **Buk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buk](https://vinkius.com/mcp/buk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
