# SugarCRM (Enterprise CRM & Customer Success API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sugarcrm-enterprise-crm-customer-success-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sugarcrm-enterprise-crm-customer-success-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sugarcrm-enterprise-crm-customer-success-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage SugarCRM records, relationships, and customer data directly from your AI agent.

## Description
Connect your **SugarCRM** instance to any AI agent to streamline your customer success and sales operations. This server provides a comprehensive set of tools to interact with your CRM data using natural language.

### What you can do

- **Record Management** — List, create, retrieve, update, and delete records across any SugarCRM module (Accounts, Contacts, Leads, etc.)
- **Relationship Mapping** — List related records and manage links between different entities to understand the full customer journey
- **Advanced Filtering** — Query specific data using complex JSON filters to find exactly what you need
- **Data Analytics** — Count records matching specific criteria to generate quick reports and insights
- **Bulk Operations** — Handle complex workflows with support for bulk requests and relationship management

### How it works

1. Subscribe to this server
2. Provide your SugarCRM Instance URL, Username, and Password
3. Start managing your enterprise CRM data from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Teams** — quickly update lead statuses and log interactions without leaving your workflow
- **Customer Success Managers** — retrieve account history and related contacts instantly
- **Data Analysts** — query and count records across modules for rapid reporting


## Available Tools
- **bulk_request**: Execute multiple API calls in a single request
- **count_records**: Count records matching a filter in a module
- **create_record**: Create a new record in a SugarCRM module
- **delete_record**: Delete a specific SugarCRM record
- **get_record**: Retrieve a specific SugarCRM record by ID
- **link_record**: Create a relationship to an existing record
- **list_records**: g., Accounts, Contacts). Supports complex filtering via JSON.

List filtered records for a specific SugarCRM module
- **list_related_records**: List related records for a specific link
- **unlink_record**: Remove a relationship between records
- **update_record**: Update an existing SugarCRM record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SugarCRM (Enterprise CRM & Customer Success API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 5 accounts from SugarCRM."

**🤖 AI Agent:**
> I've retrieved the first 5 accounts. They include 'Nelson Inc', 'Global Tech', and 'Apex Corp'. Would you like to see the details for any of these?

---

**👤 You:**
> "Count how many Leads we have in the system."

**🤖 AI Agent:**
> There are currently 1,250 leads recorded in your SugarCRM instance.

---

**👤 You:**
> "Show me all contacts related to Account ID 'acc_123'."

**🤖 AI Agent:**
> I've found 3 contacts related to that account: John Doe, Jane Smith, and Robert Brown. Do you need the contact info for any of them?


## Installation & Usage

To install and use the **SugarCRM (Enterprise CRM & Customer Success API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sugarcrm-enterprise-crm-customer-success-api](https://vinkius.com/mcp/sugarcrm-enterprise-crm-customer-success-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
