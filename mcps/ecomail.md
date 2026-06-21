# Ecomail MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecomail)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ecomail-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ecomail-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage email campaigns, track subscribers, and monitor marketing automation via the Ecomail API.

## Description
Integrate **Ecomail**, the powerful marketing automation and email platform, directly into your AI workflow. Manage your email campaigns and templates, track contact lists and individual subscriber profiles, monitor automation results, and oversee your marketing operations using natural language.

### What you can do

- **Campaign Oversight** — List and retrieve detailed information and performance metrics for all your email marketing campaigns.
- **Subscriber Intelligence** — Monitor contact address lists, individual profiles, and subscription statuses across your organization.
- **Automation Monitoring** — Track marketing automation programs and campaign delivery results to ensure effective engagement.
- **Marketing Auditing** — Retrieve high-level summaries of list volumes, campaign activity, and account limits instantly.

### How it works

1. Connect the Ecomail integration to your AI assistant.
2. Authorize using your Ecomail API Key (found in your account settings).
3. Orchestrate your marketing automation and subscriber management through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check campaign open rates and list volumes on the go.
- **CRM Specialists** — Research subscriber profiles and list memberships via chat during segmentation.
- **Operations Teams** — Monitor campaign execution and marketing metadata across the organization instantly.


## Available Tools
- **get_ecomail_account_metadata**: Retrieve metadata and usage limits for your Ecomail account
- **get_campaign_performance_details**: Get detailed information and metrics for a specific email campaign
- **quick_marketing_volume_audit**: Retrieve a high-level summary of campaign and list activity
- **get_subscriber_profile**: Get full profile and history for a specific subscriber by email
- **list_marketing_address_lists**: List all contact address lists configured in your Ecomail account
- **list_email_marketing_campaigns**: List all email campaigns
- **list_latest_marketing_campaigns**: Identify the most recently created or sent campaigns
- **list_address_list_subscribers**: List all subscribers within a specific address list
- **list_email_templates**: List all available email message templates
- **search_marketing_subscribers**: Search for subscribers using a keyword or email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ecomail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email marketing campaigns."

**🤖 AI Agent:**
> I've found several campaigns, including 'Spring Sale 2024', 'Welcome series', and 'Monthly Newsletter'. Would you like to see the performance metrics for the Spring Sale?

---

**👤 You:**
> "Show me the subscribers in list '12345'."

**🤖 AI Agent:**
> List '12345' (Master Newsletter) has 500 subscribers. Recent additions include 'john.doe@example.com' and 'alice.smith@example.org'. Should I research the profile for John Doe?

---

**👤 You:**
> "Which email templates are available for use?"

**🤖 AI Agent:**
> You have 5 active templates, including 'Standard Promo', 'Transactional Receipt', and 'Blog Update'. Would you like the unique ID for any of these templates?


## Installation & Usage

To install and use the **Ecomail** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecomail](https://vinkius.com/mcp/ecomail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
