# Apex27 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apex27)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/apex27-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/apex27-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Manage letting agency operations with property listings, tenant applications, and maintenance tracking built for estate agents.

## Description
Connect your **Apex27** real estate management account to any AI agent and simplify how you coordinate listings, customer viewings, and property offers through natural conversation.

### What you can do

- **Property Management** — List all real estate listings and retrieve detailed metadata, pricing, and availability status.
- **Viewing Coordination** — Schedule and track property viewings for applicants and maintain an organized viewing diary.
- **Offer Tracking** — List and record new financial offers on properties to manage your sales pipeline effectively.
- **CRM & Contacts** — Manage your directory of applicants, vendors, and landlords with full contact history support.
- **Maintenance & Tasks** — List work orders and manage CRM appointments to keep your agency operations running smoothly.
- **Agent Insights** — Retrieve your agent profile details and verify account configurations directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Apex27 Subdomain and API Key (found in your account settings)
3. Start managing your real estate business from Claude, Cursor, or any MCP client

### Who is this for?

- **Estate Agents** — quickly retrieve property details and schedule viewings via simple AI commands.
- **Agency Managers** — monitor offer progress and verify team appointments directly from the workspace.
- **Operations Teams** — track work orders and manage the contact directory via the AI assistant.


## Available Tools
- **create_contact**: Add a new contact to Apex27
- **record_offer**: Record a new offer on a property
- **schedule_viewing**: Schedule a new property viewing
- **get_me**: Get agent account information
- **get_property_details**: Get details of a specific property
- **list_appointments**: List CRM appointments
- **list_contacts**: List contacts (applicants, vendors, etc.)
- **list_offers**: List property offers
- **list_properties**: List real estate properties
- **list_viewings**: List property viewings
- **list_work_orders**: List maintenance work orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apex27** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active property listings in my account."

**🤖 AI Agent:**
> I've retrieved your property listings. You have 5 active properties including '2-bed Flat in Chelsea', 'Luxury Villa in Marbella', and 'Commercial Unit A'. Which one would you like more details on?

---

**👤 You:**
> "Schedule a viewing for 'John Doe' (ID: cont_1029) for property 'prop_8823' on Dec 1st at 10 AM."

**🤖 AI Agent:**
> Viewing scheduled! I've booked the appointment for John Doe to see property prop_8823 on 2024-12-01 at 10:00 AM UTC. The agent and landlord have been notified in Apex27.

---

**👤 You:**
> "Show me all recent offers for the 'Luxury Villa'."

**🤖 AI Agent:**
> I've fetched the offers. For the 'Luxury Villa' (ID: prop_5521), there are 2 recent offers: $1.2M from 'Sarah Smith' and $1.15M from 'International Investments'. Shall I retrieve the status for either of them?


## Installation & Usage

To install and use the **Apex27** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apex27](https://vinkius.com/mcp/apex27)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
