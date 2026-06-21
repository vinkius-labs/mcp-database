# Albi Restoration MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/albi-restoration)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/albi-restoration-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/albi-restoration-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage restoration projects from damage assessment through job completion with tools built for contractors and adjusters.

## Description
Connect your **Albi** (albiware.com) account to any AI agent and take full control of your restoration contracting and project management workflows through natural conversation.

### What you can do

- **Project Lifecycle Orchestration** — List and manage all restoration projects programmatically, retrieving detailed high-fidelity statuses, staff assignments, and timelines in real-time
- **Financial Insights & KPIs** — Programmatically retrieve project-specific financial data, including high-fidelity revenue metrics, costs, and gross margins directly through your agent
- **Relationship Management Architecture** — Access and manage your entire database of individual contacts, clients, and business organizations to maintain a perfectly coordinated ecosystem
- **Inventory & Asset Tracking** — Programmatically track physical equipment and specialized restoration gear to oversee your organization's assets and availability efficiently
- **Operational Monitoring** — Access project activities, monitor active webhooks, and verify API connectivity directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Albi settings (Settings > Integrations)
3. Start orchestrating your restoration business from Claude, Cursor, or any MCP client

No more manual logging into field service apps or digging through complex financial spreadsheets. Your AI acts as your dedicated project coordinator and business analyst.

### Who is this for?

- **Restoration Contractors** — instantly retrieve project summaries and update statuses using natural language commands
- **Project Managers** — monitor staff assignments and track financial KPIs across multiple sites without leaving your workspace
- **Operations Leads** — automate the oversight of organization-wide inventory and contact directories through simple AI queries


## Available Tools
- **check_api_health**: Verify Albi API status
- **create_new_contact**: Add a new contact
- **create_new_restoration_project**: Requires project name and primary contact.

Start a new project
- **get_project_financial_kpis**: Retrieve financial KPIs for a project
- **get_project_details**: Get details for a specific project
- **list_project_activities**: List all tasks and activities
- **list_restoration_contacts**: List all contacts
- **list_inventory_equipment**: List assets and equipment
- **list_restoration_organizations**: List all organizations
- **list_restoration_projects**: List all restoration projects
- **list_defined_project_roles**: List available project roles
- **list_configured_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Albi Restoration** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active restoration projects in Albi."

**🤖 AI Agent:**
> I've retrieved your active projects. You currently have 3 projects in progress, including 'Water Damage - Main St' (ID: proj_123) and 'Fire Restoration'. Would you like the detailed high-fidelity status for any of these?

---

**👤 You:**
> "What are the financial KPIs for project 'proj_123'?"

**🤖 AI Agent:**
> Accessing financial intelligence... For project proj_123, current revenue is $15,400 with total costs of $8,200, resulting in a high-fidelity gross margin of 46.7%. Need help checking the project activities?

---

**👤 You:**
> "Check my inventory for available dehumidifiers."

**🤖 AI Agent:**
> Retrieving equipment list... You currently have 12 dehumidifiers in stock and 5 deployed on active job sites. All assets are within high-fidelity tracking parameters. Shall I list your available air movers?


## Installation & Usage

To install and use the **Albi Restoration** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/albi-restoration](https://vinkius.com/mcp/albi-restoration)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
