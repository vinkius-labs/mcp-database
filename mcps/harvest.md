# Harvest MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harvest)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/harvest-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/harvest-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate time tracking and invoicing via Harvest — manage clients, invoices, and time entries directly from any AI agent.

## Description
Connect your **Harvest** account to any AI agent and take full control of your time tracking, client management, and invoicing through natural conversation.

### What you can do

- **Time Tracking Oversight** — List and inspect tracked time entries to monitor team productivity.
- **Client Management** — List all clients, create new ones, and update company details effortlessly.
- **Invoicing Automation** — Access your invoice history, create new drafts, and manage billing statuses.
- **Project Monitoring** — List all active projects and retrieve detailed information for each.
- **User Profile** — Get information about the current authenticated user and account status.
- **Operational Efficiency** — Use AI to identify unbilled time or upcoming invoice deadlines across your organization.

### How it works

1. Subscribe to this server
2. Enter your Harvest Access Token and Account ID
3. Start managing your time and billing from Claude, Cursor, or any MCP-compatible client

No more manual exporting of time reports. Your AI assistant acts as a dedicated Billing Coordinator or Operations Manager.

### Who is this for?

- **Project Managers** — instantly retrieve project time summaries and client details during status calls.
- **Operations Leaders** — automate the oversight of invoicing and time entry compliance.
- **Freelancers & Small Agencies** — manage your entire billing cycle and time tracking without leaving your communication flow.


## Available Tools
- **delete_client**: Permanently delete a client
- **create_client**: Create a new client in Harvest
- **create_invoice**: Create a new invoice for a client
- **get_client**: Get detailed information for a specific client
- **get_invoice**: Get details for a specific invoice
- **get_my_profile**: Get information about the current authenticated user
- **list_clients**: List all clients in your Harvest account
- **list_invoices**: List all invoices, including drafts and sent ones
- **list_projects**: List all projects in the account
- **list_time_entries**: List tracked time entries
- **update_client**: Update an existing client name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harvest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all time entries from last week."

**🤖 AI Agent:**
> I've retrieved your time entries. Last week, your team logged a total of 120 hours across 5 projects. The most active project was 'Cloud Migration' with 45 hours. Would you like a detailed breakdown by user?

---

**👤 You:**
> "Create a new client named 'Acme Corp'."

**🤖 AI Agent:**
> Client created! I've successfully added 'Acme Corp' (ID: 8821) to your Harvest account. Should I associate a new project with this client now?

---

**👤 You:**
> "Show me all active projects."

**🤖 AI Agent:**
> Accessing projects... You have 4 active projects: 'Website Redesign', 'Mobile App Support', 'Internal Ops', and 'Q2 Marketing'. Which one would you like to see time summaries for?


## Installation & Usage

To install and use the **Harvest** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harvest](https://vinkius.com/mcp/harvest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
