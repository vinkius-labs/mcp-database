# WorkWave MCP Server

Manage service orders, customer accounts, and field technicians on WorkWave — the field service management platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/workwave)

## Overview
**Category:** customer-support
**Tools Count:** 10

## Description
Connect your **WorkWave Service** account to any AI agent and manage your field service operations through natural conversation.

### What you can do

- **Service Orders** — Browse and list all work requests, retrieve full details for specific orders, and update lifecycle statuses (e.g., InProgress, Completed)
- **Customer Accounts** — List all field service accounts and retrieve comprehensive details including contact info, billing history, and service locations
- **Field Personnel** — List all registered technicians and field staff, and retrieve profile details to check roles, skills, and contact info
- **Equipment Inventory** — Monitor and audit managed assets and equipment used across your field service operations directly from your agent
- **Site Discovery** — Retrieve physical service locations and job site addresses, including geographical coordinates for routing purposes
- **Operational Insights** — Quickly find unique account, order, employee, and location IDs required for automated field service workflows
- **Health Monitoring** — Verify the connectivity and status of your WorkWave API integration to ensure real-time data sync

### How it works

1. Subscribe to this server
2. Enter your WorkWave API Key
3. Start managing your field operations through Claude, Cursor, or any MCP-compatible client

No more manual digging through complex dispatching dashboards to check a job status. Your AI agent becomes your field service coordinator.

### Who is this for?

- **Dispatchers & Schedulers** — monitor job queues and update service order statuses through simple chat commands
- **Operations Managers** — audit customer accounts, verify technician profiles, and manage equipment inventory without manual navigation
- **Service Technicians** — quickly lookup order details and site locations while on the go through conversation
- **Customer Support Teams** — retrieve account billing history and service status to provide rapid assistance to field customers


## Available Tools
- **get_account_details**: Retrieves details for a specific customer account
- **get_api_health**: Checks the health and connectivity of the WorkWave API integration
- **get_employee_profile**: Retrieves profile details for a specific employee
- **get_order_details**: Retrieves details for a specific service order
- **list_field_service_accounts**: Lists customer accounts in the WorkWave Service platform
- **list_field_employees**: Lists technicians and field staff registered in WorkWave
- **list_service_equipment**: Lists managed equipment and assets used in field service
- **list_service_locations**: Lists physical service locations and job sites
- **list_service_orders**: Lists service orders and work requests
- **update_order_status**: g. mark as Pending, InProgress, or Completed).

Updates the lifecycle status of a service order


## Installation & Usage

To install and use the **WorkWave** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workwave](https://vinkius.com/mcp/workwave)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
