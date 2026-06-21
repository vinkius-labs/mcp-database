# GitScrum ClientFlow MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitscrum-clientflow)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gitscrum-clientflow-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gitscrum-clientflow-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Streamline client operations via GitScrum ClientFlow — manage clients, create invoices, draft proposals, and monitor project budgets directly from any AI agent.

## Description
### What you can do

- **Client management** — list, inspect, and create client records with contact details and project history
- **Invoice generation** — create and review invoices linked to client accounts with line items and totals
- **Proposal drafting** — browse existing proposals and their approval statuses for any client
- **Budget monitoring** — check project budget consumption and remaining allocations in real-time
- **Dashboard insights** — access the ClientFlow dashboard for a consolidated view of revenue and client activity
- **Time billing** — list and log time entries on tasks for accurate client billing

### How it works

1. Subscribe to the GitScrum ClientFlow integration from the marketplace
2. Enter your GitScrum API token and company slug
3. Ask your agent to review client portfolios, draft invoices, or check budget health — works in Claude, Cursor, and any MCP client

Your agent becomes your client operations assistant, eliminating context-switching between billing and project tools.

### Who is this for?

- **Agency owners** — monitor all client budgets and revenue from a single conversational interface
- **Project managers** — track billable hours and generate invoices without leaving the workflow
- **Finance teams** — review proposals, invoices, and budget consumption in natural language


## Available Tools
- **project_budget**: Get project budget
- **create_client**: Create a new client
- **get_client**: Get client details
- **list_clients**: List all clients
- **clientflow_dashboard**: Get ClientFlow dashboard overview
- **create_invoice**: Pass additional fields as JSON in the body parameter.

Create an invoice for a client
- **get_invoice**: Get invoice details
- **list_invoices**: List all invoices
- **get_proposal**: Get proposal details
- **list_proposals**: List all proposals
- **log_time**: Log time on a task
- **list_time_entries**: List time tracking entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitScrum ClientFlow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our clients on GitScrum."

**🤖 AI Agent:**
> You have 6 active clients: 1) 'TechCorp Inc.' (3 active projects, $24,500 invoiced), 2) 'Design Studio LLC' (1 project, $8,200 invoiced), 3) 'StartupXYZ' (2 projects, $15,300 invoiced)... Would you like to see invoices for any specific client?

---

**👤 You:**
> "Show me the ClientFlow dashboard overview."

**🤖 AI Agent:**
> ClientFlow Dashboard: Total revenue this month: $47,800 (+12% vs last month). 4 pending invoices worth $12,400. 2 proposals awaiting approval ($18,000 combined). 3 projects at >80% budget consumption. Shall I drill into any of these areas?

---

**👤 You:**
> "Create a new client 'Acme Corp' with email billing@acme.com."

**🤖 AI Agent:**
> Client 'Acme Corp' created successfully with billing contact billing@acme.com. The client UUID is c8d9e0f1-2345-6789-abcd-ef0123456789. Ready to create a proposal or invoice for this client?


## Installation & Usage

To install and use the **GitScrum ClientFlow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitscrum-clientflow](https://vinkius.com/mcp/gitscrum-clientflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
