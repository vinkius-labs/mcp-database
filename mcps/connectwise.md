# ConnectWise MCP Server

Equip your AI to seamlessly manage ConnectWise PSA tickets, clients, and technical documentation via text.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/connectwise)

## Overview
**Category:** customer-support
**Tools Count:** 9

## Description
Empower your conversational AI with deep integration into **ConnectWise Manage (PSA)**. Enhance technical support operations by enabling your agent to triage issues, update existing service tickets, and retrieve critical client environment data without leaving your conversational interface.

### What you can do

- **Ticketing Operations** — Rapidly inspect queue statuses, assign incoming tickets, or update internal notes naturally.
- **Asset & Configuration Retrieval** — Look up devices, configurations, and agreements associated with a specific managed client.
- **Billing & Time Entries** — Log billable technical time or adjust status workflows directly through the chat.

### How it works

1. Attach the ConnectWise tool to your preferred MCP interface.
2. Supply your designated Company ID, Public Key, and Private Key for secure authentication.
3. Chat seamlessly with your agent to govern your helpdesk and IT services.

### Who is this for?

- **Level 1/2 Support Technicians** — Quickly triage, update notes, and close straightforward tickets without bogging down in complex UI menus.
- **Service Delivery Managers** — Audit ticket lifecycles, check SLA compliance, and monitor board queues efficiently.
- **MSP Owners** — Pull immediate reports on client profitability or check current active incidents directly from a mobile chat.


## Available Tools
- **create_ticket**: Create a new service ticket in ConnectWise Manage
- **get_company**: Returns name, contact info, territory, and status.

Retrieve detailed information about a specific company
- **get_ticket**: Returns summary, priority, status, assigned member, and notes.

Retrieve detailed information about a specific service ticket
- **list_sales_activities**: Retrieve a list of sales and service activities
- **list_companies**: Use to discover company identifiers for ticket creation.

Retrieve a list of companies/clients in ConnectWise
- **list_contacts**: Use to find external contact details.

Retrieve a list of individual contacts within companies
- **list_members**: Retrieve a list of internal staff members
- **list_service_tickets**: Supports pagination via pageSize.

Retrieve a list of service tickets from ConnectWise Manage
- **search_tickets_by_summary**: Useful for finding tickets by keyword.

Find service tickets matching a keyword in the summary


## Installation & Usage

To install and use the **ConnectWise** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/connectwise](https://vinkius.com/mcp/connectwise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
