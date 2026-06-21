# MailboxPower MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailboxpower)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mailboxpower-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mailboxpower-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Delight contacts with personalized physical gifts, greeting cards, and direct mail sent automatically from your CRM.

## Description
Connect your **MailboxPower** account to any AI agent and manage direct mail marketing through natural conversation.

### What you can do

- **Gift Sending** — Send personalized gifts, cards, and promotional items
- **Campaign Management** — Create and manage direct mail campaigns
- **Product Catalog** — Browse available products, cards, and promotional items
- **Delivery Tracking** — Monitor shipment status and delivery confirmations
- **Contact Management** — Manage recipient lists and contact information

### How it works

1. Subscribe to this server
2. Enter your MailboxPower API Key
3. Start sending mail from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — send personalized gifts to prospects
- **Marketing** — run direct mail campaigns with tracking
- **Customer Success** — send thank-you cards and retention gifts


## Available Tools
- **add_contact_to_automation**: Start an automation for a contact
- **add_contact_to_group**: Add a contact to a group
- **create_contact**: Create a new contact
- **create_group**: Create a new group
- **get_contact**: Get contact details
- **list_automations**: List all automations
- **list_contacts**: List all contacts
- **list_groups**: List all contact groups
- **send_shipment**: Send a card or gift


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MailboxPower** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show the product catalog and send a thank-you card to a client."

**🤖 AI Agent:**
> Catalog: 45 products. Cards (12): Thank You ($3.50), Birthday ($4.00), Holiday ($4.50). Gifts: Coffee Mug ($15), Gift Box ($35), Premium Basket ($75). Promo: Branded Pen ($5), Notebook ($12). Card sent! ✅ Thank You card to Sarah Chen, 123 Main St, NY 10001. Message: 'Thank you for your partnership!' Est. delivery: May 1-3.

---

**👤 You:**
> "Create a gift campaign for the top 10 clients."

**🤖 AI Agent:**
> Campaign created! 'Q2 Client Appreciation'. Recipients: 10 top clients. Product: Premium Gift Box ($35 each). Total: $350 + $45 shipping. Personal message: 'Thank you for being an amazing partner!' Schedule: Ships May 1. Estimated delivery: May 3-6. Status: Pending approval. ⬜ Approve to send.

---

**👤 You:**
> "Show delivery status for all active campaigns and contact lists."

**🤖 AI Agent:**
> Active campaigns: 2. 'Spring Appreciation' (25 gifts, 22 delivered ✅, 3 in transit). 'New Client Welcome' (8 cards, 8 delivered ✅). Delivery rate: 100% (no returns). Avg delivery: 3.1 days. Contact lists: 3. 'Top Clients' (25), 'New Clients Q2' (14), 'Partners' (8). Total contacts: 47.


## Installation & Usage

To install and use the **MailboxPower** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailboxpower](https://vinkius.com/mcp/mailboxpower)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
