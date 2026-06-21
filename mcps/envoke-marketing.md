# Envoke Marketing MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/envoke-marketing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/envoke-marketing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/envoke-marketing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage email campaigns, track contact lists, and monitor performance via the Envoke API.

## Description
Integrate **Envoke**, the powerful and intuitive email marketing and communication platform, directly into your AI workflow. Manage your email campaigns and contact lists, track individual subscriber profiles and interaction history, monitor real-time performance statistics, and oversee your automated marketing operations using natural language.

### What you can do

- **Campaign Oversight** — List and retrieve detailed information, subject lines, and current statuses for all your email marketing campaigns.
- **Contact Intelligence** — Monitor contact address lists and individual profile details, resolving subscription statuses and custom field values.
- **Performance Monitoring** — Access real-time campaign telemetry, resolving sent, open, and click-through counts via chat.
- **Marketing Auditing** — Retrieve high-level summaries of list volumes, campaign activity, and organizational account health instantly.

### How it works

1. Connect the Envoke integration to your AI assistant.
2. Authorize using your Envoke API ID and API Key (found in your account settings).
3. Orchestrate your email marketing and subscriber management through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check campaign open rates and subscriber counts on the go.
- **Communication Specialists** — Research contact profiles and list memberships via chat during campaign planning.
- **Operations Teams** — Monitor marketing volumes and organizational Envoke metadata instantly.


## Available Tools
- **get_envoke_account_metadata**: Retrieve metadata and limits for your Envoke account
- **get_campaign_performance_stats**: Get performance statistics for a specific email campaign
- **get_campaign_details**: Get detailed settings and status for a specific email campaign
- **get_contact_profile**: Get full profile and history for a specific contact
- **quick_marketing_volume_audit**: Retrieve a high-level summary of campaign activity and list counts
- **list_contact_address_lists**: List all contact lists configured in your account
- **list_email_campaigns**: List all email marketing campaigns in your Envoke account
- **list_marketing_contacts**: List all contacts registered in your organization
- **list_successfully_sent_campaigns**: Identify campaigns that have already been sent to subscribers
- **search_contacts_by_email**: Search for a contact using their email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Envoke Marketing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns."

**🤖 AI Agent:**
> I've found 5 active campaigns, including 'Monthly Newsletter' and 'Q2 Lead Magnet'. The Monthly Newsletter has already been sent to 3,500 contacts. Would you like to see the performance stats?

---

**👤 You:**
> "Show me the performance for campaign ID 12345."

**🤖 AI Agent:**
> Campaign ID 12345 has 3,500 sends, 850 opens (24.3%), and 240 clicks (6.8%). Status is 'Completed'. Should I check for any delivery bounces?

---

**👤 You:**
> "Search for contact 'alex@example.com'."

**🤖 AI Agent:**
> Alex is currently 'Subscribed' and a member of 2 lists: 'General Announcements' and 'Product Beta'. Their last recorded click was on March 15th. Should I pull their full interaction history?


## Installation & Usage

To install and use the **Envoke Marketing** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/envoke-marketing](https://vinkius.com/mcp/envoke-marketing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
