# Mailjet MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailjet)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mailjet-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mailjet-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Send transactional emails and manage marketing campaigns via the Mailjet REST API.

## Description
Connect your **Mailjet** account to any AI agent to automate your transactional messaging and email marketing workflows. This MCP server enables your agent to send emails using the v3.1 Send API, manage subscriber lists, and track campaign performance directly from natural language interfaces.

### What you can do

- **Transactional Delivery** — Send single or batch emails with full support for HTML, attachments, and variables
- **Audience Management** — List all contacts, create new subscriber records, and manage contact lists (address books)
- **Subscription Control** — Add or remove contacts from specific lists and manage opt-in statuses programmatically
- **Campaign Tracking** — List historical campaigns and retrieve real-time performance statistics (opens, clicks, bounces)
- **Metadata Oversight** — Fetch detailed configuration and status for any campaign or subscriber collection

### How it works

1. Subscribe to this server
2. Enter your Mailjet API Public Key and Secret Key
3. Start managing your communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — Monitor campaign results and manage subscriber segments via simple natural language commands
- **Developers** — Quickly test email delivery and verify list logic directly from your IDE
- **Operations Teams** — Automate the synchronization of contact data and audit delivery performance effortlessly


## Available Tools
- **add_contact_to_list**: Requires list ID and contact ID/Email.

Subscribe a contact to a specific list
- **get_campaign_performance**: Get performance statistics for a campaign
- **create_new_contact**: Requires at least an Email address.

Add a new contact to the database
- **get_campaign_details**: Get details for a specific campaign
- **list_marketing_campaigns**: List all campaigns
- **list_subscriber_lists**: List all contact lists
- **list_all_contacts**: List all contacts in the Mailjet account
- **send_transactional_email**: Requires a JSON body matching Mailjet v3.1 Send API structure.

Send an email using Mailjet Send API v3.1


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailjet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a transactional email to 'passenger@example.com' with subject 'Boarding Pass'."

**🤖 AI Agent:**
> I've sent the email. The message has been queued by Mailjet. You can track the delivery status using the campaign tools.

---

**👤 You:**
> "List all active contact lists in my Mailjet account."

**🤖 AI Agent:**
> I've retrieved your contact lists. You have 3 active lists: 'Newsletter Subscribers', 'Product Updates', and 'Transactional Users'.

---

**👤 You:**
> "Show performance stats for campaign ID '12345'."

**🤖 AI Agent:**
> I've fetched the statistics. For campaign 12345, you have an open rate of 22.5% and a click rate of 3.2% across 5,000 recipients.


## Installation & Usage

To install and use the **Mailjet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailjet](https://vinkius.com/mcp/mailjet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
