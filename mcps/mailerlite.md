# MailerLite MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailerlite)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mailerlite-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mailerlite-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your email marketing campaigns, subscribers, and automation via MailerLite.

## Description
Empower your AI agent to orchestrate your entire email marketing ecosystem with **MailerLite**, the simple yet powerful platform for growing your business. By connecting MailerLite to your agent, you transform complex subscriber management into a natural conversation. Your agent can instantly list active subscribers, create targeted groups, and audit campaign performance without you ever touching a dashboard. Whether you are managing a small newsletter or a large-scale marketing operation, your agent acts as a real-time marketing manager, ensuring your communication is always precise and effective.

### What you can do

- **Subscriber Management** — List, retrieve, create, and update subscribers using email or ID to keep your list healthy.
- **Groups & Segments** — Organize your audience into targeted groups and segments for highly personalized marketing.
- **Campaign Insights** — List sent and draft campaigns to stay on top of your marketing efforts and audit content.
- **Form Tracking** — Monitor your popups and embedded forms to understand lead generation performance in real-time.
- **Account Auditing** — Quickly retrieve account details and authorized access to maintain organizational control.

### How it works

1. Subscribe to this server
2. Enter your MailerLite API Token
3. Start managing your email marketing through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — instantly retrieve campaign statuses and subscriber counts without opening the MailerLite app.
- **Customer Support Teams** — verify subscriber details and group memberships directly from the support chat.
- **Content Creators** — check if new newsletters have been correctly drafted and scheduled for distribution.
- **Operations Leads** — automate audience querying to orchestrate cross-functional marketing teams smoothly.


## Available Tools
- **add_subscriber_to_group**: Add a subscriber to a group
- **create_group**: Create a new subscriber group
- **create_subscriber**: Mandatory: email is required.

Create or update a MailerLite subscriber
- **delete_subscriber**: Delete a MailerLite subscriber
- **get_me**: Get MailerLite account details
- **get_subscriber**: Get details for a specific subscriber
- **list_campaigns**: List MailerLite campaigns
- **list_forms**: Default is popup.

List MailerLite forms
- **list_groups**: List all MailerLite groups
- **list_segments**: List all MailerLite segments
- **list_subscribers**: Supports filtering by status (active, unsubscribed, unconfirmed, bounced, junk).

List MailerLite subscribers
- **remove_subscriber_from_group**: Remove a subscriber from a group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MailerLite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 active subscribers in MailerLite."

**🤖 AI Agent:**
> I've retrieved your recent subscribers. You have 5 new active members, including 'john@doe.com' and 'jane@smith.net'. Would you like the full details for any of them?

---

**👤 You:**
> "Show me all my subscriber groups."

**🤖 AI Agent:**
> I've found 3 subscriber groups in your account: 'VIP Customers', 'Newsletter Leads', and 'Event Attendees'. Which group would you like to inspect?

---

**👤 You:**
> "Check if there are any sent campaigns this week."

**🤖 AI Agent:**
> I've scanned your campaigns. You have 2 sent campaigns this week: 'Weekly Update #42' and 'Flash Sale October'. I can provide performance metrics for both if needed.


## Installation & Usage

To install and use the **MailerLite** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailerlite](https://vinkius.com/mcp/mailerlite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
