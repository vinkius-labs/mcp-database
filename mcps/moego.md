# MoeGo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moego)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/moego-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/moego-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your pet care business via MoeGo — track appointments, pets, and customers directly from your AI agent.

## Description
Connect your **MoeGo** pet care business account to your AI agent and streamline your grooming and boarding operations through natural conversation.

### What you can do

- **Appointment Management** — List all scheduled appointments and get detailed status updates.
- **Pet & Customer Profiles** — View registered pets, their owners, and specific care details including breeds and ages.
- **Service & Staff Oversight** — Access your catalog of grooming services and list of active staff members.
- **Scheduling** — Create new service appointments for pets and customers with simple commands.
- **Reputation Monitoring** — Retrieve recent customer reviews and feedback directly within your chat.
- **Business Configuration** — Access general metadata and settings for your MoeGo account.
- **Deep Inspection** — Fetch complete metadata for specific appointments or pets using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your MoeGo API Key
3. Start managing your pet business from Claude, Cursor, or any MCP client

### Who is this for?

- **Pet Groomers & Boarders** — quickly check the day's schedule or look up a pet's details without opening the MoeGo app.
- **Business Owners** — monitor operations, staff, and client growth directly from your communication tools.
- **Receptionists** — verify appointment times and customer info while multitasking.


## Available Tools
- **create_appointment**: Schedule a new appointment
- **get_appointment**: Get appointment details
- **get_business_settings**: Get business configuration
- **get_pet**: Get specific pet details
- **list_appointments**: List grooming appointments
- **list_customers**: List MoeGo customers
- **list_pets**: ) associated with your business.

List all registered pets
- **list_reviews**: List customer reviews
- **list_services**: List grooming services
- **list_staff**: List business staff


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MoeGo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's grooming schedule."

**🤖 AI Agent:**
> I've retrieved today's schedule. You have 6 appointments: 'Buddy' (Golden Retriever) at 10:00 AM, 'Luna' (Persian Cat) at 11:30 AM, and 4 more in the afternoon. Would you like the contact details for Buddy's owner?

---

**👤 You:**
> "Get details for the pet with ID pet_123."

**🤖 AI Agent:**
> Inspecting pet_123... This is 'Max', a 3-year-old Beagle. He weighs 12kg and his owner is Sarah Jenkins. Max has a note: 'Sensitive skin, use hypoallergenic shampoo'. Shall I check his last appointment date?

---

**👤 You:**
> "List all our available grooming services and prices."

**🤖 AI Agent:**
> I've fetched your service catalog. You offer 12 services, including 'Full Grooming - Large Dog' ($85.00), 'Puppy's First Bath' ($45.00), and 'Nail Trim' ($15.00). Would you like to check which staff members are assigned to these services?


## Installation & Usage

To install and use the **MoeGo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moego](https://vinkius.com/mcp/moego)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
