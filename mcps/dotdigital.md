# Dotdigital MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dotdigital)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dotdigital-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dotdigital-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage email campaigns, track contacts, and monitor marketing automation via the Dotdigital API.

## Description
Integrate **Dotdigital**, the powerful marketing automation and omnichannel platform, directly into your AI workflow. Manage your email campaigns and templates, track contact address books and individual profiles, monitor automation programs (journeys), and oversee your marketing operations using natural language.

### What you can do

- **Campaign Oversight** — List and retrieve detailed information and subject lines for all your email marketing campaigns.
- **Contact Intelligence** — Monitor contact address books, individual profile details, and subscription statuses across your organization.
- **Automation Monitoring** — Track active marketing automation programs and customer journeys to ensure effective engagement.
- **Marketing Auditing** — Retrieve high-level summaries of address book volumes, campaign activity, and account limits instantly.

### How it works

1. Connect the Dotdigital integration to your AI assistant.
2. Authorize using your Dotdigital API Username and Password (found in your account settings).
3. Orchestrate your marketing automation and contact management through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check campaign statuses and address book volumes on the go.
- **CRM Administrators** — Research contact profiles and subscription history via chat during segmentation.
- **Automation Leads** — Monitor program execution and marketing metadata across the organization instantly.


## Available Tools
- **get_dotdigital_account_metadata**: Retrieve metadata and limits for your Dotdigital account
- **get_campaign_details**: Get detailed information for a specific email campaign
- **get_contact_profile**: Get full profile and history for a specific contact by email
- **quick_marketing_health_audit**: Retrieve a high-level summary of campaign and contact activity
- **list_marketing_address_books**: List all contact address books configured in your Dotdigital account
- **list_email_campaigns**: List all email marketing campaigns
- **list_address_book_contacts**: List all contacts within a specific address book
- **list_automation_programs**: List all active marketing automation programs (journeys)
- **list_email_templates**: List all available email message templates
- **search_marketing_contacts**: Search for contacts using a specific query string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dotdigital** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email campaigns."

**🤖 AI Agent:**
> I've found several campaigns, including 'Q3 Newsletter', 'Flash Sale - August', and 'Welcome Series'. Would you like to see the subject line for the Q3 Newsletter?

---

**👤 You:**
> "Show me the contacts in address book '12345'."

**🤖 AI Agent:**
> Address book '12345' (VIP Customers) contains 150 contacts. Recent additions include 'john.doe@example.com' and 'jane.smith@example.org'. Should I research the profile for John Doe?

---

**👤 You:**
> "Which marketing automation programs are currently active?"

**🤖 AI Agent:**
> The currently active programs include 'Abandoned Cart Recovery', 'Post-Purchase Upsell', and 'Annual Anniversary Series'. All are in an 'Active' state. Would you like to see the start date for the Abandoned Cart program?


## Installation & Usage

To install and use the **Dotdigital** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dotdigital](https://vinkius.com/mcp/dotdigital)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
