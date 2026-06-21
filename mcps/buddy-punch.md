# Buddy Punch MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buddy-punch)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/buddy-punch-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/buddy-punch-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track employee hours with GPS-verified clock-ins, PTO management, and payroll-ready timesheet exports your team will love.

## Description
Connect your **Buddy Punch** (Enterprise) account to any AI agent and take full control of your workforce time tracking and automated payroll workflows through natural conversation.

### What you can do

- **Punch Orchestration** — Programmatically perform high-fidelity punch-in and punch-out actions for employees, including adding descriptive metadata and shift notes in real-time
- **Workforce Visibility** — List and manage employee profiles and administrative settings programmatically to maintain a perfectly coordinated organizational structure
- **Time Entry Intelligence** — Retrieve detailed high-fidelity time cards and entry history by pay period to coordinate payroll data collection directly through your agent
- **Schedule Monitoring** — Access and monitor work schedules and published shift updates to oversee team distribution and labor capacity efficiently
- **Pay Cycle Management** — Retrieve complete directories of defined pay periods and historical cycles to maintain high-fidelity financial records

### How it works

1. Subscribe to this server
2. Retrieve your **Subscription Key** from the Buddy Punch Developer Hub (Enterprise plan required)
3. Start managing your team's attendance and schedules from Claude, Cursor, or any MCP client

No more manual chasing of missing time cards or digging through complex shift tables. Your AI acts as your dedicated workforce administrator and payroll coordinator.

### Who is this for?

- **HR Managers** — instantly retrieve employee time summaries and log manual punches using natural language commands
- **Operations Leads** — monitor team shift distribution and verify clock-in accuracy without leaving your workspace
- **Payroll Specialists** — automate the collection of structured time entry data for internal reporting through simple AI queries


## Available Tools
- **create_employee**: Create a new employee
- **list_employees**: List all employees
- **list_pay_periods**: List pay periods
- **list_work_schedules**: List work schedules
- **list_time_entries**: List time entries
- **punch_in_out**: Perform a punch action


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buddy Punch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active employees in my Buddy Punch account."

**🤖 AI Agent:**
> I've retrieved your employee directory. You currently have 15 active staff members, including 'John Doe' (ID: 1024) and 'Jane Smith'. Would you like to check the current punch status for any of them?

---

**👤 You:**
> "Punch in employee '1024' with the note 'Starting early morning shift'."

**🤖 AI Agent:**
> Punch complete! I've successfully recorded a 'Punch In' for employee 1024 at 7:55 AM. The shift note has been added to their time card. Shall I check their scheduled end time?

---

**👤 You:**
> "Show the time entries for the current pay period."

**🤖 AI Agent:**
> Fetching pay period data... For the current cycle, your team has logged a total of 480 hours. Highlights include 40 hours from 'John Doe' and 38 from 'Jane Smith'. Would you like the high-fidelity break metadata?


## Installation & Usage

To install and use the **Buddy Punch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buddy-punch](https://vinkius.com/mcp/buddy-punch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
