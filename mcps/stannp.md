# Stannp MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stannp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/stannp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/stannp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate direct mail and physical letters via Stannp — manage letters, postcards, and campaigns directly from any AI agent.

## Description
Connect your **Stannp** account to any AI agent and simplify your direct mail marketing, physical letter delivery, and mailing list management through natural conversation.

### What you can do

- **Physical Mail Delivery** — Create and send single or bulk letters and postcards programmatically directly from your agent
- **Campaign Management** — Query all configured direct mail campaigns and retrieve detailed metadata and status
- **Recipient Control** — Query your database of contacts and mailing addresses to choose the right recipients for each piece
- **Account tracking** — Access your real-time account balance to manage your mailing spend
- **Live Monitoring** — Access a history of sent and drafted letters to stay on top of your physical outreach

### How it works

1. Subscribe to this server
2. Enter your Stannp API Key from your account settings
3. Start managing your direct mail from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_postcard**: Create and send a postcard
- **create_recipient**: Create a new mailing recipient
- **get_campaign**: Get details for a direct mail campaign
- **get_letter**: Get details for a specific letter
- **get_recipient**: Get details for a specific recipient
- **create_physical_letter**: Send a physical letter
- **get_account_balance**: Check account credit balance
- **list_direct_mail_campaigns**: List direct mail campaigns
- **list_letters**: List sent and drafted letters
- **list_postcards**: List sent and drafted postcards
- **list_mailing_recipients**: List mailing recipients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stannp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my sent letters in Stannp."

**🤖 AI Agent:**
> I've retrieved your letters. You have 10 sent items, including 'Welcome Pack' and 'Invoice #123'.

---

**👤 You:**
> "Show me all direct mail campaigns with their delivery status and response rates."

**🤖 AI Agent:**
> 8 direct mail campaigns. Active (3): "Spring Promo Postcards" (2,340 sent, 2,280 delivered, 98 responses, 4.3% response rate, QR scans: 156). "VIP Thank You Letters" (120 sent, 118 delivered, personalized). "Re-engagement Mailer" (890 sent, in transit). Completed (4): avg 3.8% response rate. Draft (1): "Summer Sale Flyer" (ready for review). Total pieces mailed this month: 5,200. Total spend: £1,890. Average cost per piece: £0.36. Best performing: "Holiday Catalog" at 6.2% response.

---

**👤 You:**
> "Create and send a personalized postcard to our top 50 customers with a loyalty discount code."

**🤖 AI Agent:**
> Postcard campaign created: "VIP Loyalty Reward". Recipients: 50 top customers (by lifetime value). Personalization: first name, unique discount code per recipient (VIP-[NAME]-20). Design: A5 size, full-color front with product image, personalized back with message and QR code to redemption page. Print status: queued for next business day. Estimated delivery: 3-5 business days. Cost: £22.50 (£0.45/piece). Tracking: Royal Mail tracked. Redemption tracking: unique codes linked to CRM profiles.


## Installation & Usage

To install and use the **Stannp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stannp](https://vinkius.com/mcp/stannp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
