# Giddyup MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/giddyup)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/giddyup-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/giddyup-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Coordinate field service teams with job dispatching, route optimization, and real-time status updates for mobile workforces.

## Description
Connect your **Giddyup** account to any AI agent and take full control of your roofing and construction workflows through natural conversation.

### What you can do

- **Lead Orchestration** — List and manage potential customer records programmatically, including contact info and acquisition metadata
- **Job Lifecycle** — Monitor active roofing and construction projects and retrieve detailed technical metadata and status in real-time
- **Customer Intelligence** — Access your complete customer directory and retrieve detailed profiles to streamline field coordination
- **Operational Visibility** — Get a comprehensive overview of your construction pipeline using natural language commands
- **Field Coordination** — Access granular details for specific jobs to ensure your team has the latest project requirements

### How it works

1. Subscribe to this server
2. Retrieve your **API Authentication Key** from your Giddyup settings (Custom Application Integration)
3. Start managing your construction CRM from Claude, Cursor, or any MCP client

No more manual toggling between project spreadsheets. Your AI acts as your dedicated construction operations coordinator.

### Who is this for?

- **Project Managers** — instantly check job statuses and retrieve customer requirements using natural language
- **Sales Teams** — manage lead queues and update contact details without leaving your workspace
- **Operations Leaders** — monitor the entire construction pipeline and identify bottlenecks through automated queries


## Available Tools
- **check_giddyup_status**: Verify connectivity
- **create_job**: Create a job
- **create_lead**: Create a lead
- **get_customer**: Get customer details
- **get_job**: Get job details
- **get_lead**: Get lead details
- **list_customers**: List customers
- **list_invoices**: List invoices
- **list_jobs**: List jobs
- **list_leads**: List leads
- **list_users**: List technicians
- **update_job**: Update a job
- **update_lead**: Update a lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Giddyup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active roofing jobs in Giddyup."

**🤖 AI Agent:**
> I've retrieved your active projects. You currently have 5 ongoing jobs, including 'Maple St. Residence' and 'Oak Blvd. Commercial'. Would you like the detailed status for any of these?

---

**👤 You:**
> "Show me the latest 3 leads collected this week."

**🤖 AI Agent:**
> Scanning leads... I've found 3 new entries from this week: 'John Doe' (Residential), 'Sarah Smith' (Repair), and 'Acme Corp' (Inspection). Which one should I provide contact info for?

---

**👤 You:**
> "Get details for job ID 'J-12345'."

**🤖 AI Agent:**
> Fetching job J-12345... This project is for 'Pine Road Apartments'. It's currently in the 'Production' stage with the crew assigned. The estimated completion date is next Friday. Should I check for any pending tasks?


## Installation & Usage

To install and use the **Giddyup** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/giddyup](https://vinkius.com/mcp/giddyup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
