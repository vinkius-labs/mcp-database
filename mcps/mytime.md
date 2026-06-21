# MyTime MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mytime)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mytime-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mytime-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage business operations via MyTime — track appointments, staff, and services directly from your AI agent.

## Description
Connect your **MyTime** partner account to your AI agent and take control of your business operations and scheduling through natural conversation.

### What you can do

- **Appointment Management** — List all scheduled appointments and get detailed status updates and customer info.
- **Staff Oversight** — Access a complete list of staff members and their associated roles.
- **Service & Product Catalog** — View all services and retail products offered by your business.
- **Real-time Availability** — Check available time slots for specific staff members and services.
- **Customer Insights** — List and search your customer database for easy profile lookup.
- **Reputation Monitoring** — Retrieve recent customer reviews and feedback.
- **Multi-Location Support** — Manage operations across all your business branches.

### How it works

1. Subscribe to this server
2. Enter your MyTime Partner API Key and (Optional) Subdomain
3. Start managing your business from Claude, Cursor, or any MCP client

### Who is this for?

- **Business Owners** — quickly check the day's schedule or verify staff availability without opening the MyTime portal.
- **Operations Managers** — monitor service performance and customer growth directly from your chat.
- **Support Teams** — verify appointment details and customer history during assistance.


## Available Tools
- **get_appointment**: Get specific appointment details
- **get_availability**: Check staff availability
- **get_business_info**: Get high-level business info
- **list_appointments**: List scheduled appointments
- **list_customers**: List business customers
- **list_locations**: List business locations
- **list_products**: List retail products
- **list_reviews**: List customer reviews
- **list_services**: List available services
- **list_staff**: List staff members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MyTime** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's appointment schedule."

**🤖 AI Agent:**
> I've retrieved today's schedule. You have 6 appointments: 3 for Haircuts, 2 for Manicures, and 1 for a Consultation. Shall I give you the details for the first one?

---

**👤 You:**
> "Check if staff member 'John Doe' is available for a 'Full Massage' this Friday."

**🤖 AI Agent:**
> Searching availability... John Doe has 3 open slots this Friday: 10:00 AM, 1:30 PM, and 4:00 PM. Would you like to see the customer details for anyone on his waitlist?

---

**👤 You:**
> "List all our retail products and prices."

**🤖 AI Agent:**
> I've fetched your product catalog. You have 15 items in stock, including 'Premium Shampoo' ($25.00), 'Argan Oil' ($30.00), and others. Shall I check the current inventory levels for any of these?


## Installation & Usage

To install and use the **MyTime** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mytime](https://vinkius.com/mcp/mytime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
