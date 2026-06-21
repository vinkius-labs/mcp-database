# MailWizz MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailwizz)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mailwizz-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mailwizz-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage email marketing campaigns and subscriber lists via the MailWizz REST API.

## Description
Connect your **MailWizz** instance to any AI agent to automate your professional email marketing and audience management. This MCP server enables your agent to manage subscriber lists, control campaign lifecycles, and update subscriber data directly from natural language interfaces.

### What you can do

- **Campaign Oversight** — List all email campaigns and retrieve detailed metadata and status information
- **Mailing Control** — Pause or unpause campaigns and manage their delivery lifecycle programmatically
- **Audience Management** — List all subscriber collections (lists) and retrieve their unique identifiers
- **Subscriber Administration** — Add, update, and remove subscribers from specific lists using their UIDs
- **Data Ingestion** — Sync subscriber information and manage custom fields across your email databases
- **Self-Hosted Support** — Works with any self-hosted MailWizz instance using your personal API keys

### How it works

1. Subscribe to this server
2. Enter your MailWizz API URL and Public Key
3. Start managing your marketing audience from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — Monitor campaign results and manage subscriber segments via simple natural language commands
- **CRM Specialists** — Quickly update contact information and audit list health without leaving your productivity tools
- **Developers** — Integrate MailWizz's robust marketing logic into your custom internal tools


## Available Tools
- **add_subscriber_to_list**: Requires a list UID and subscriber data.

Add a new subscriber to a list
- **list_email_campaigns**: List all email marketing campaigns
- **delete_list_subscriber**: Remove a subscriber from a list
- **get_campaign_details**: Get details for a specific campaign
- **get_list_details**: Get details for a specific subscriber list
- **list_list_subscribers**: List subscribers in a specific list
- **list_subscriber_collections**: List all subscriber lists
- **pause_email_campaign**: Pause a running campaign
- **update_list_subscriber**: Update an existing subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MailWizz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active email campaigns in MailWizz."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 5 campaigns, including 'Product Launch Q4 (UID: sb123abc)', 'Monthly Update', and 'Re-engagement Flow'. Which one would you like to see metadata for?

---

**👤 You:**
> "Add 'user@example.com' to my 'Main Leads' list (UID: 'lz987xyz')."

**🤖 AI Agent:**
> Successfully added user@example.com to the list Main Leads. The subscriber UID is 'sub-abc-123' and they are now ready to receive your mailings.

---

**👤 You:**
> "Pause the email campaign with UID 'cp456def'."

**🤖 AI Agent:**
> I've triggered the pause command for campaign cp456def. MailWizz has updated the status and sending is now suspended.


## Installation & Usage

To install and use the **MailWizz** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailwizz](https://vinkius.com/mcp/mailwizz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
