# Finch MCP Server

Connect Finch to automate HRIS and Payroll integration — list employees, retrieve employment data, and manage pay statements directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/finch)

## Overview
**Category:** human-resources
**Tools Count:** 11

## Description
Finch is the unified API for HRIS and payroll. This MCP server allows your AI agent to interact with various HR and payroll providers through a single integration flawlessly.

### Key Features
- **Directory Orchestration** — List all employees in the connected organization and fetch detailed profiles natively.
- **Employment Intelligence** — Retrieve granular employment data including job titles, departments, and compensation flawlessly.
- **Payroll Transparency** — Access pay groups and individual pay statements to monitor payroll data synchronously.
- **Connection Introspection** — Check the status, provider, and authorized permissions for any connection flawlessly native.
- **Automated Job Tracking** — Monitor data sync jobs to ensure your HRIS data is always up to date flawlessly through the agent.
- **Provider Discovery** — List all supported HRIS and payroll providers to verify integration compatibility flawlessly.

### How it works
1. Subscribe to this server
2. Enter your Finch Access Token (obtained via Finch Connect)
3. Start managing your HRIS and payroll data from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **HR Operations** — automate employee data retrieval and verification without manual portal exports
- **Finance Teams** — monitor payroll statements and compensation data directly from your chat workflow
- **Product Teams** — integrate unified HR data into your internal tools and workflows through simple natural language queries


## Available Tools
- **get_automated_job**: Get details for a specific automated job
- **get_company**: Get organization data (legal name, EIN, primary address)
- **get_employment**: Get employment data for an individual (title, salary, department, etc.)
- **get_individual**: Get personal data for an individual (name, email, SSN, etc.)
- **get_me**: Get details for the authorized application/user connection
- **introspect**: Check the status and permissions of the current connection
- **list_automated_jobs**: List automated data sync jobs
- **list_directory**: Read the employee directory for the connected organization
- **list_pay_groups**: List pay groups for the organization
- **list_pay_statements**: List pay statements for a specific payment ID
- **list_supported_providers**: List all HRIS/Payroll providers supported by Finch


## Installation & Usage

To install and use the **Finch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/finch](https://vinkius.com/mcp/finch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
