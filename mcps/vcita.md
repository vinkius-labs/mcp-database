# vCita MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vcita)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vcita-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vcita-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Run your small business with online scheduling, payment collection, and client management that keeps everything in one place.

## Description
Connect your **vCita** business management account to any AI agent and simplify how you coordinate your schedule, client records, and billing through natural conversation.

### What you can do

- **Client Management** — List, search, and create new client records in your CRM with full metadata support.
- **Appointment Scheduling** — Book new services, list upcoming appointments, and cancel existing bookings instantly via AI.
- **Service Catalog** — Query your offered services and prices to understand your bookable offering.
- **Financial Tracking** — Monitor your cash flow by listing invoices, payments, and price estimates sent to clients.
- **Team Coordination** — List staff members and their roles to manage your business directory.
- **Operational Visibility** — Check account status and connection health to ensure your business engine is running smoothly.

### How it works

1. Subscribe to this server
2. Enter your vCita API Token (found in your developer portal or settings)
3. Start managing your business operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Service Providers & Freelancers** — quickly book appointments and check client payment statuses via simple AI commands.
- **Small Business Owners** — monitor invoices and manage the client directory directly from the workspace.
- **Operations Managers** — coordinate staff availability and track billing history via the AI assistant.


## Available Tools
- **cancel_appointment**: Cancel booking
- **create_new_booking**: Schedule a service
- **create_crm_client**: Add new customer
- **get_api_status**: Get account status
- **get_client_details**: Get client info
- **list_staff_members**: List team users
- **list_scheduled_appointments**: List bookings
- **list_crm_clients**: List CRM customers
- **list_price_estimates**: List client estimates
- **list_client_invoices**: List all invoices
- **list_recorded_payments**: List transactions
- **list_offered_services**: List bookable services


## 💬 Prompt Examples

Here are some examples of how you can interact with the **vCita** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my upcoming appointments for this week."

**🤖 AI Agent:**
> I've retrieved your schedule. You have 3 appointments: 'Consultation' with John Doe (Tue, 10 AM), 'Strategy Session' with Jane Smith (Wed, 2 PM), and 'Follow-up' with Mike Ross (Fri, 9 AM). Which one would you like more details on?

---

**👤 You:**
> "Search for a client with the email 'jane.doe@example.com'."

**🤖 AI Agent:**
> I've found the record. Jane Doe (ID: cl_10293) is a registered client. She has one outstanding invoice for $150 and an upcoming appointment on Wednesday. Shall I retrieve her full contact history?

---

**👤 You:**
> "Book a 'New Consultation' for client 'cl_10293' on Dec 1st at 10 AM."

**🤖 AI Agent:**
> Booking successful! I've scheduled the 'New Consultation' (Service ID: svc_552) for client cl_10293 on 2024-12-01 at 10:00 AM UTC. A confirmation has been sent to the client.


## Installation & Usage

To install and use the **vCita** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vcita](https://vinkius.com/mcp/vcita)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
