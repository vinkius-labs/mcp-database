# Handwrytten MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/handwrytten)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/handwrytten-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/handwrytten-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate handwritten notes via Handwrytten — manage cards, fonts, and send physical mail directly from any AI agent.

## Description
Connect your **Handwrytten** account to any AI agent and take full control of your physical outreach and relationship management through natural conversation.

### What you can do

- **Card Selection** — Browse and list all available stationery and card categories for any occasion.
- **Font Management** — List and select from various realistic handwriting styles to personalize your notes.
- **Order Automation** — Send single or bulk handwritten cards with personalized messages directly from the chat.
- **Address Book Access** — Manage your saved recipients and retrieve address details for quick sending.
- **Credit Monitoring** — Instantly check your account credit balance to manage your outreach budget.
- **Template Insights** — Browse your message templates to maintain brand consistency in your physical mail.

### How it works

1. Subscribe to this server
2. Enter your Handwrytten API Key (found in Settings > API Keys)
3. Start sending handwritten notes from Claude, Cursor, or any MCP-compatible client

No more manual data entry or ordering through the web interface. Your AI assistant acts as a dedicated outreach coordinator or relationship manager.

### Who is this for?

- **Sales & Marketing Teams** — automate personalized follow-ups and high-touch outreach campaigns.
- **Customer Success Managers** — send 'Thank You' or 'Birthday' cards to clients without leaving the CRM flow.
- **Executive Assistants** — manage the sending of physical holiday or appreciation cards effortlessly.


## Available Tools
- **get_credit_balance**: Check current account credit balance
- **get_order**: Get details for a specific order
- **list_address_book**: List recipients in your address book
- **list_cards**: List all available cards/stationery
- **list_categories**: List all card categories
- **list_fonts**: List all available handwriting fonts
- **list_gifts**: List available gifts that can be included with cards
- **list_orders**: List history of card orders
- **list_templates**: List message templates
- **send_card**: Requires card_id, font_id, message, and recipient details.

Send a single handwritten card


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Handwrytten** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a 'Thank You' card to John Doe using font hwDavid."

**🤖 AI Agent:**
> I've started the process. I found 3 'Thank You' cards. Which one would you like to use? After that, I'll need the recipient's address to complete the order.

---

**👤 You:**
> "Check my current credit balance."

**🤖 AI Agent:**
> Accessing account... Your current Handwrytten balance is $145.50. This is enough to send approximately 35 more premium cards. Would you like to see your recent order history?

---

**👤 You:**
> "List all available handwriting fonts."

**🤖 AI Agent:**
> Retrieving fonts... Handwrytten offers 25+ styles, including: 'hwDavid' (Clean Print), 'hwCursive' (Classic Cursive), 'hwCasual' (Relaxed), and 'hwProfessional'. Would you like a description of any specific style?


## Installation & Usage

To install and use the **Handwrytten** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/handwrytten](https://vinkius.com/mcp/handwrytten)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
