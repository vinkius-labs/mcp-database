# Berg System CRM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/berg-system-crm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/berg-system-crm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/berg-system-crm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Close more deals with a CRM built for financial advisors that tracks client relationships, policies, and follow-ups.

## Description
Connect your **Berg System** account to any AI agent and take full control of your insurance agency operations and customer relationship workflows through natural conversation.

### What you can do

- **Customer Orchestration** — List and search through individual and corporate client directories programmatically, retrieving detailed high-fidelity profile metadata and contact history
- **Sales Pipeline Intelligence** — Monitor sales opportunities and track deal progress across your entire agency to maintain a perfectly coordinated sales cycle
- **Insurance Policy Monitoring** — Retrieve active insurance policies and access high-fidelity document metadata directly through your agent to oversee coverage status
- **Infrastructure Monitoring** — Access system employee lists and manage CRM-related tasks programmatically for instant operational reporting
- **Relationship Intelligence** — Retrieve complete historical interactions for any record to maintain high-fidelity oversight of your agency's relationship ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **Tenant ID** and **OAuth Access Token** from your Berg System instance
3. Start managing your insurance business from Claude, Cursor, or any MCP client

No more manual toggling between CRM tabs or digging through paper policy files. Your AI acts as your dedicated agency administrator and sales coordinator.

### Who is this for?

- **Insurance Agents** — instantly retrieve client coverage details and update lead statuses using natural language commands
- **Agency Managers** — monitor team productivity and track agency-wide sales trends without leaving your workspace
- **Operations Leads** — automate the oversight of corporate client directories and task management through simple AI queries


## Available Tools
- **check_api_health**: Verify Berg System API status
- **create_new_company**: Add a new business client
- **create_new_customer**: Supports forceAdd to bypass duplicates.

Add a new customer
- **get_customer_details**: Get details for a customer
- **get_sales_custom_fields**: Retrieve custom sales fields
- **list_crm_companies**: List corporate clients
- **list_crm_customers**: List CRM customers
- **list_stored_documents**: List uploaded documents
- **list_system_employees**: List organization employees
- **list_insurance_policies**: List active insurance policies
- **list_sales_opportunities**: List sales records
- **list_crm_tasks**: List active tasks and reminders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Berg System CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active insurance policies for client 'John Doe'."

**🤖 AI Agent:**
> I've retrieved John Doe's profile. He currently has 2 active policies: 'Auto Platinum' (ID: pol_123) and 'Home Secure'. Would you like the high-fidelity coverage metadata for these?

---

**👤 You:**
> "Show my recent sales opportunities in Berg System."

**🤖 AI Agent:**
> Accessing pipeline... I found 5 recent opportunities including a high-value Life Insurance lead from 'Acme Corp' and 4 other prospects. Shall I retrieve the high-fidelity transaction history?

---

**👤 You:**
> "Create a new lead for 'Alice Smith' (alice@example.com) interested in 'Life Insurance'."

**🤖 AI Agent:**
> Lead created! I've successfully registered Alice Smith in your CRM and tagged her as interested in Life Insurance (ID: lead_789). Shall I assign a follow-up task to a specific agent?


## Installation & Usage

To install and use the **Berg System CRM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/berg-system-crm](https://vinkius.com/mcp/berg-system-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
