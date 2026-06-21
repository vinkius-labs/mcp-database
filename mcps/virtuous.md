# Virtuous MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/virtuous)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/virtuous-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/virtuous-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage nonprofit fundraising and donor relationships via Virtuous — list contacts, track individuals, manage gifts, and oversee projects directly from any AI agent.

## Description
Connect your **Virtuous** CRM to any AI agent and take full control of your nonprofit's donor management and fundraising workflows through natural conversation.

### What you can do

- **Contact Management** — List and retrieve detailed information for households, organizations, and foundations.
- **Individual Tracking** — Manage specific people within donor contacts, including creating and updating their profiles.
- **Gift & Contribution Tracking** — Query financial contributions, list recent gifts, and record new donations directly into the system.
- **Project Oversight** — List and inspect specific fundraising projects to track progress and allocation.
- **Custom Field Access** — Retrieve metadata for contact and individual custom fields to ensure data consistency.

### How it works

1. Subscribe to this server
2. Enter your Virtuous API Key
3. Start managing your donor database from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Development Directors** — quickly pull donor histories and gift records without navigating complex CRM menus.
- **Nonprofit Admins** — automate the creation of new contacts and individuals during outreach campaigns.
- **Data Analysts** — query project and gift data to generate instant reports on fundraising performance.


## Available Tools
- **create_contact**: Create a new contact
- **create_gift**: Create a new gift
- **create_individual**: Create a new individual
- **create_project**: Create a new project
- **delete_contact**: Delete a contact
- **get_contact**: Retrieve a specific contact by ID
- **get_gift**: Retrieve a specific gift by ID
- **get_individual**: Retrieve a specific individual by ID
- **get_project**: Retrieve a specific project by ID
- **list_contact_custom_fields**: List custom fields for contacts
- **list_contacts**: List all contacts (households, organizations, foundations)
- **list_gifts**: List all gifts
- **list_individual_custom_fields**: List custom fields for individuals
- **list_individuals**: List all individuals
- **list_projects**: List all projects
- **update_contact**: Update an existing contact
- **update_gift**: Update an existing gift
- **update_individual**: Update an existing individual


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Virtuous** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 contacts from our Virtuous database."

**🤖 AI Agent:**
> I've retrieved the first 10 contacts. They include households like 'The Smith Family' (ID: 402) and organizations like 'Global Giving Foundation' (ID: 882). Would you like details on a specific one?

---

**👤 You:**
> "Show me the details for gift ID 12345."

**🤖 AI Agent:**
> Fetching gift 12345... This was a $500.00 contribution from Contact ID 992, processed on October 12th for the 'Clean Water Initiative' project.

---

**👤 You:**
> "What are the active fundraising projects?"

**🤖 AI Agent:**
> I found 3 active projects: 'Annual Gala 2024', 'Community Housing Fund', and 'Education Scholarship'. Which one would you like to inspect?


## Installation & Usage

To install and use the **Virtuous** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/virtuous](https://vinkius.com/mcp/virtuous)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
