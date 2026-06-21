# Urbanise MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/urbanise)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/urbanise-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/urbanise-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage strata and community properties with owner portals, meeting management, and financial reporting for property managers.

## Description
Connect your **Urbanise** property management account to any AI agent and simplify how you coordinate building operations, financial records, and community engagement through natural conversation.

### What you can do

- **Property Management** — List all property plans and retrieve detailed metadata for your managed ecosystem.
- **Occupant & Strata Support** — List residents and owners to manage communications and community directories.
- **Maintenance Control** — Create, list, and track maintenance jobs and facility tasks directly from your agent.
- **Financial Visibility** — Query ledger data, billing records, and property budgets to stay on top of your accounts.
- **Supply Chain** — List managed suppliers and service providers associated with your property plans.
- **Asset Tracking** — Monitor building equipment and infrastructure assets managed in the FM module.

### How it works

1. Subscribe to this server
2. Enter your Urbanise Region, Client ID, and Access Token
3. Start managing your properties and facility maintenance from Claude, Cursor, or any MCP client

### Who is this for?

- **Property Managers** — quickly retrieve occupant lists and verify property budgets via simple AI commands.
- **Facility Managers** — schedule maintenance jobs and track asset health directly from the workspace.
- **Strata Management Companies** — coordinate supplier lists and monitor financial ledgers for entire property portfolios.


## Available Tools
- **check_api_health**: Verify Urbanise API connectivity
- **create_maintenance_job**: Requires job title and description.

Schedule a new maintenance task
- **get_client_profile**: Get authenticated client details
- **list_facility_assets**: List infrastructure equipment
- **list_property_budgets**: List budgets for plans
- **list_financial_data**: Retrieve ledger and billing info
- **list_maintenance_jobs**: List facility maintenance tasks
- **list_accounting_ledgers**: List chart of accounts
- **list_property_occupants**: List residents and owners
- **list_property_plans**: List all property plans
- **list_managed_suppliers**: List property suppliers
- **list_configured_webhooks**: List active event webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Urbanise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all property plans managed in my Urbanise account."

**🤖 AI Agent:**
> I've retrieved your property plans. You have 5 active plans including 'Sunset Heights', 'Business Park Tower', and 'Central Strata'. Which one would you like to inspect?

---

**👤 You:**
> "Show me all active maintenance jobs for 'Sunset Heights'."

**🤖 AI Agent:**
> I've fetched the maintenance list. There are 3 active jobs for 'Sunset Heights': 'Elevator Inspection', 'Pool Cleaning', and 'HVAC Filter Change'. Shall I check the status of any specific task?

---

**👤 You:**
> "Create a maintenance job: 'Fix leaking pipe in Room 402'."

**🤖 AI Agent:**
> Success! The maintenance job 'Fix leaking pipe in Room 402' has been created in the FM module with ID JOB-10293. I'll let you know once a supplier is assigned.


## Installation & Usage

To install and use the **Urbanise** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/urbanise](https://vinkius.com/mcp/urbanise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
