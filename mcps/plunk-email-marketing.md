# Plunk Email Marketing MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plunk-email-marketing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/plunk-email-marketing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/plunk-email-marketing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate your email marketing via Plunk — send transactional emails, track events, and manage contacts.

## Description
Connect your AI agent to **Plunk**, the versatile email marketing platform designed for developers. This integration allows you to manage your audience, send transactional messages, and track user behavioral events directly through natural conversation.

### What you can do

- **Audience Management** — List, create, and update contacts in your Plunk database, including subscription states
- **Transactional Emails** — Send HTML emails to users for notifications, alerts, or onboarding directly via the agent
- **Event Tracking** — Log custom user actions to trigger automated workflows or segment your audience
- **Campaign & Template Oversight** — List your saved templates and monitor the status of your marketing campaigns
- **Lifecycle Control** — Seamlessly delete contacts or update metadata based on user feedback

### How it works

1. Subscribe to this server
2. Enter your **Plunk Secret Key** (found in your Plunk project settings)
3. Start automating your communication flows via chat

### Who is this for?

- **Growth Marketers** — quickly send test emails or check audience segments
- **Product Managers** — track user events and audit email templates without leaving the conversation
- **Customer Support** — update contact metadata or send direct notifications to users


## Available Tools
- **create_or_update_contact**: Provide metadata as a JSON string if needed.

Create a new contact or update an existing one
- **delete_contact**: Permanently delete a contact from your audience
- **get_contact_details**: Get comprehensive information for a specific contact
- **list_email_campaigns**: Retrieve a list of all email marketing campaigns
- **list_contacts**: Retrieve all contacts in your Plunk audience
- **list_email_templates**: Retrieve a list of all saved email templates
- **send_transactional_email**: Send a transactional email to one or more recipients
- **track_user_event**: Provide data as a JSON string.

Track a custom action performed by a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plunk Email Marketing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts in my Plunk audience."

**🤖 AI Agent:**
> Retrieving contacts... I found several users, including 'john@example.com' (Subscribed) and 'jane@example.com' (Unsubscribed).

---

**👤 You:**
> "Send a welcome email to 'test@example.com'."

**🤖 AI Agent:**
> Sending transactional email... Done! The welcome message has been successfully queued for 'test@example.com' with subject 'Welcome to our platform!'.


## Installation & Usage

To install and use the **Plunk Email Marketing** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plunk-email-marketing](https://vinkius.com/mcp/plunk-email-marketing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
