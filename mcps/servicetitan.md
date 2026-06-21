# ServiceTitan MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/servicetitan)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/servicetitan-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/servicetitan-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage field service operations via ServiceTitan — track customers, jobs, appointments, and inventory directly from any AI agent.

## Description
Connect your **ServiceTitan** account to any AI agent to streamline your field service management. Access customer data, manage job dispatches, update appointments, and track inventory through natural conversation.

### What you can do

- **Customer & Location Management** — List and create customers and locations within the CRM module.
- **Job Dispatching** — Retrieve job details and manage active dispatches from the Dispatch module.
- **Appointment Updates** — Update appointment statuses in real-time to keep your team in sync.
- **Accounting & Payments** — List invoices and record payments directly within the Accounting module.
- **Inventory Control** — Monitor SKUs and create inventory adjustments to keep stock levels accurate.

### How it works

1. Subscribe to this server
2. Enter your ServiceTitan Client ID, Client Secret, and Tenant ID
3. Start managing your field operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — quickly check job statuses and dispatch schedules without leaving your workflow.
- **Accounting Teams** — track invoices and record payments without switching between multiple browser tabs.
- **Inventory Managers** — adjust stock levels and monitor SKUs directly from the chat interface.


## Available Tools
- **create_inventory_adjustment**: Adjust stock levels in ServiceTitan
- **create_customer**: Create a new customer in ServiceTitan
- **create_payment**: Record a payment in ServiceTitan
- **list_customers**: List customers in ServiceTitan
- **list_invoices**: List invoices in ServiceTitan
- **list_jobs**: Retrieve job details in ServiceTitan
- **list_locations**: List locations in ServiceTitan
- **list_skus**: List inventory items (SKUs) in ServiceTitan
- **update_appointment**: Update appointment status in ServiceTitan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ServiceTitan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customers in our ServiceTitan account."

**🤖 AI Agent:**
> I've retrieved the customer list. You have several active records, including 'John Doe' (ID: 4567) and 'Jane Smith' (ID: 8901). Would you like to see more details for a specific customer?

---

**👤 You:**
> "Update appointment ID 98765 to status 'Completed'."

**🤖 AI Agent:**
> The appointment 98765 has been successfully updated to 'Completed' in the Dispatch module.

---

**👤 You:**
> "Show me the current inventory SKUs."

**🤖 AI Agent:**
> Fetching inventory... I found several items including 'Copper Pipe 1/2 inch' (SKU: CP-12) and 'Thermostat Model X' (SKU: TH-X). Do you need to adjust stock levels for any of these?


## Installation & Usage

To install and use the **ServiceTitan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/servicetitan](https://vinkius.com/mcp/servicetitan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
