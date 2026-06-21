# Nimble CRM (Social Sales CRM & Contacts API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nimble-crm-social-sales-crm-contacts-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nimble-crm-social-sales-crm-contacts-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nimble-crm-social-sales-crm-contacts-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage your Nimble CRM contacts and user profile directly through AI — list, retrieve, and manage social sales data seamlessly.

## Description
Connect your **Nimble CRM** account to any AI agent to streamline your social sales and contact management workflows through natural conversation.

### What you can do

- **User Profile** — Retrieve details about your authenticated Nimble account and credentials.
- **Contact Discovery** — List and search for contacts using keywords, tags, and custom filters to find the right leads.
- **Deep Contact Inspection** — Fetch full metadata, social profiles, and detailed data for specific contacts using their unique IDs.
- **Database Cleanup** — Delete contacts based on advanced search queries to keep your CRM organized and up to date.

### How it works

1. Subscribe to this server
2. Enter your Nimble API Access Token
3. Start managing your contacts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — quickly find contact details and social profiles without switching between tabs.
- **Marketing Managers** — filter and list contacts by tags to organize outreach campaigns.
- **Operations Leads** — automate CRM maintenance and data cleanup through simple AI commands.


## Available Tools
- **delete_contacts**: Delete Nimble contacts
- **get_contact**: Get details for specific Nimble contacts
- **get_myself**: Get current Nimble user details
- **list_contacts**: List Nimble contacts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nimble CRM (Social Sales CRM & Contacts API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my Nimble user profile details."

**🤖 AI Agent:**
> I've retrieved your profile. You are logged in as 'Alex Rivera' (ID: 54321) with the email alex@company.com. Your account is currently active.

---

**👤 You:**
> "Search for contacts tagged as 'Lead' with the keyword 'Software'."

**🤖 AI Agent:**
> I found 3 contacts matching your criteria. The top results are 'Jordan Smith' from TechSoft and 'Casey Lee' from SoftSystems. Would you like the details for any of them?

---

**👤 You:**
> "Get all information for contact ID 5f4e3d2c1b."

**🤖 AI Agent:**
> Inspecting contact 5f4e3d2c1b... This is 'Morgan Blake', Senior VP at GlobalCorp. I've found their LinkedIn profile, Twitter handle, and primary work phone number.


## Installation & Usage

To install and use the **Nimble CRM (Social Sales CRM & Contacts API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nimble-crm-social-sales-crm-contacts-api](https://vinkius.com/mcp/nimble-crm-social-sales-crm-contacts-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
