# Smaily MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smaily-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/smaily-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/smaily-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing campaigns, subscribers, and automations directly through Smaily.

## Description
Connect your **Smaily** account to any AI agent and take full control of your email marketing workflows through natural conversation.

### What you can do

- **Subscriber Management** — List, add, update, or delete subscribers in your contact lists with ease.
- **Campaign Control** — Retrieve lists of campaigns, fetch specific details, and trigger the sending of email campaigns directly.
- **Templates & Content** — Access and inspect your email templates to ensure your messaging is always on brand.
- **Automation Workflows** — List available automated workflows and trigger them for specific subscribers to nurture leads instantly.
- **Data Insights** — Query campaign and automation data to understand your marketing performance without leaving your chat interface.

### How it works

1. Subscribe to this server
2. Enter your Smaily Subdomain, API Username, and API Password
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — quickly check campaign statuses and trigger newsletters without logging into the dashboard
- **Sales Teams** — manually add leads to specific automation workflows directly from their workflow
- **Developers** — integrate email triggers and subscriber updates into their coding environment for faster testing


## Available Tools
- **add_update_subscriber**: Add or update a Smaily subscriber
- **delete_subscriber**: Delete a Smaily subscriber
- **get_campaign**: Get details for a specific Smaily campaign
- **get_template**: Get details for a specific Smaily template
- **list_automations**: List Smaily automations
- **list_campaigns**: List Smaily campaigns
- **list_subscribers**: List Smaily subscribers
- **list_templates**: List Smaily templates
- **send_campaign**: Send a Smaily campaign
- **trigger_automation**: Trigger a Smaily automation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smaily** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current email campaigns in Smaily."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active campaigns: 'Summer Sale 2024' (ID: 101), 'Monthly Newsletter' (ID: 102), and 'Product Update' (ID: 103). Would you like details on any of these?

---

**👤 You:**
> "Add test@example.com to my subscriber list with the name 'John Doe'."

**🤖 AI Agent:**
> I've added test@example.com to your Smaily subscribers with the provided fields. The contact is now active in your list.

---

**👤 You:**
> "Trigger the welcome automation (ID: 50) for user hello@world.com."

**🤖 AI Agent:**
> Automation 50 has been successfully triggered for hello@world.com. They should receive the first email in the workflow shortly.


## Installation & Usage

To install and use the **Smaily** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smaily-alternative](https://vinkius.com/mcp/smaily-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
