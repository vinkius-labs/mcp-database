# Mailify (Sarbacane) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailify-sarbacane)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mailify-sarbacane-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mailify-sarbacane-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email and SMS marketing campaigns, address books, and contacts via the Mailify API.

## Description
Connect your **Mailify** (Sarbacane) account to any AI agent to automate your professional marketing communications. This MCP server enables your agent to manage contact lists (address books), retrieve campaign performance statistics, and update subscriber data directly from natural language interfaces.

### What you can do

- **Campaign Oversight** — List all email and SMS campaigns and retrieve detailed metadata and status information
- **Performance Auditing** — Retrieve real-time metrics including opens, clicks, and bounces for any specific campaign
- **Audience Management** — Manage multiple address books and organize your subscribers effectively
- **Contact Synchronization** — Add, update, and remove contacts from your lists programmatically
- **Metadata Inspection** — Fetch detailed configuration and settings for both campaigns and contact collections

### How it works

1. Subscribe to this server
2. Enter your Mailify (Sarbacane) API Key
3. Start managing your marketing audience from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — Monitor campaign results and manage subscriber segments via simple natural language commands
- **CRM Specialists** — Quickly update contact information and audit list health without leaving your productivity tools
- **Growth Developers** — Integrate Mailify's robust marketing logic into your custom internal dashboards


## Available Tools
- **add_contact_to_book**: Requires a list ID and contact data.

Add a new contact to an address book
- **get_campaign_performance**: Get performance statistics for a campaign
- **list_email_campaigns**: List all email marketing campaigns
- **delete_book_contact**: Remove a contact from an address book
- **get_campaign_details**: Get details for a specific campaign
- **get_address_book_details**: Get details for a specific contact list
- **list_book_contacts**: List contacts in a specific address book
- **list_address_books**: List all contact lists (address books)
- **update_book_contact**: Update an existing contact in an address book


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailify (Sarbacane)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current campaigns in Mailify."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 5 active campaigns, including 'Product Launch Q3 (ID: cp123)', 'Monthly SMS Alert', and 'Newsletter Weekly'. Would you like to see performance stats for any of them?

---

**👤 You:**
> "Show performance stats for campaign ID 'cp123'."

**🤖 AI Agent:**
> I've fetched the stats for campaign cp123. It currently has 1,250 opens (22.5%) and 145 clicks (2.6%). There were 5 bounce events recorded.

---

**👤 You:**
> "Add 'new-lead@example.com' to address book ID 'bk987'."

**🤖 AI Agent:**
> Successfully added new-lead@example.com to address book bk987. The contact ID is 'ct-abc-123' and they are now ready to receive your campaigns.


## Installation & Usage

To install and use the **Mailify (Sarbacane)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailify-sarbacane](https://vinkius.com/mcp/mailify-sarbacane)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
