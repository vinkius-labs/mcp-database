# Fieldly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fieldly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fieldly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fieldly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Connect Fieldly to automate construction management — manage work items, bookings, and invoices directly from your AI agent.

## Description
Fieldly is a specialized project management platform for the construction industry. This MCP server allows your AI agent to interact with your Fieldly account flawlessly.

### Key Features
- **Work Item Orchestration** — List all construction tasks and work items, and fetch detailed metadata natively.
- **Booking Intelligence** — Retrieve and inspect scheduling bookings to stay updated on team allocation flawlessly.
- **Invoice Management** — Access billing data and individual invoices to track project financials flawlessly.
- **Article Access** — Query your catalog of articles, materials, and service items natively.
- **Customer CRM** — Access customer profiles and contact details to manage business relationships flawlessly.
- **Identity Verification** — Verify the authorized application and user profile through the agent flawlessly.

### How it works
1. Subscribe to this server
2. Contact support@fieldly.com to enable Public API access
3. Enter your Client ID and Client Secret (found in Integration Settings)
4. Start managing your construction projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Project Managers** — monitor construction progress and task statuses without manual portal navigation
- **Operations Teams** — sync work items and material articles directly from your chat workflow
- **Site Supervisors** — quickly look up job details and team bookings through simple natural language queries


## Available Tools
- **create_work_item**: Create a new work item
- **get_booking**: Get details for a specific booking
- **get_invoice**: Get details for a specific invoice
- **get_me**: Get details for the authorized application/user
- **get_work_item**: Get details for a specific work item
- **list_articles**: List all inventory and service articles
- **list_bookings**: List all scheduling bookings
- **list_customers**: List all customers
- **list_invoices**: List all invoices
- **list_users**: List all users in the system
- **list_work_items**: List all work items (jobs/tasks)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fieldly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active work items in Fieldly."

**🤖 AI Agent:**
> I've retrieved your work items. You have 5 active projects including 'Roof Repair - Site A' (ID: 101) and 'Foundation Pumping' (ID: 102). Would you like the full details for any of these?

---

**👤 You:**
> "Show me the team bookings for tomorrow."

**🤖 AI Agent:**
> Inspecting bookings... Tomorrow you have 3 scheduled teams: 'Electricians' (8:00 AM), 'Carpenters' (10:00 AM), and 'Plumbers' (1:00 PM). Shall I list the specific site IDs for these bookings?

---

**👤 You:**
> "Check for any unpaid construction invoices."

**🤖 AI Agent:**
> Retrieving invoices... I found 2 unpaid invoices: INV-202 ($5,400) and INV-205 ($3,200). Both are associated with the 'Downtown Plaza' project. Would you like me to fetch the customer contact info?


## Installation & Usage

To install and use the **Fieldly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fieldly](https://vinkius.com/mcp/fieldly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
