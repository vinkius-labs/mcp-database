# Finch MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/finch)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/finch-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/finch-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Connect Finch to automate HRIS and Payroll integration — list employees, retrieve employment data, and manage pay statements directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Finch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the directory."

**🤖 AI Agent:**
> I've retrieved the employee directory. You have 45 individuals registered, including 'Alice Johnson' (Marketing) and 'Bob Smith' (Engineering). Would you like to see the employment details for any of them?

---

**👤 You:**
> "Check the status of my connection to Gusto."

**🤖 AI Agent:**
> Introspecting connection... Your connection to Gusto is active and authorized. You have permissions for 'directory', 'employment', and 'payment'. Shall I fetch the latest organization metadata?

---

**👤 You:**
> "List pay statements for payment ID pmt_123."

**🤖 AI Agent:**
> Retrieving pay statements... For payment pmt_123, I found statements for 12 employees. The total gross pay was $54,000. Would you like to see the individual breakdown for any specific employee?


## Installation & Usage

To install and use the **Finch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/finch](https://vinkius.com/mcp/finch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
