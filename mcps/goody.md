# Goody MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/goody)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/goody-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/goody-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate corporate gifting — browse products, send gifts, and track orders effortlessly.

## Description
Connect your **Goody** for Business account to your AI agent and streamline your corporate gifting workflows. Whether it's employee appreciation, client onboarding, or event giveaways, manage everything through simple conversation.

### What you can do

- **Gift Catalog** — Browse thousands of available gifts across various categories and price points
- **Send Gifts** — Create gift order batches and send them to one or many recipients instantly
- **Order Tracking** — Monitor the status of your gift batches and individual orders from acceptance to delivery
- **Campaign Management** — View and manage your active gifting campaigns and collections
- **Recipient History** — Keep track of everyone you've sent gifts to and their current shipment status

### How it works

1. Subscribe to this server
2. Enter your Goody API Key (found in your Goody for Business account settings)
3. Start sending and tracking gifts from Claude, Cursor, or any MCP-compatible client

No more manual data entry for every single gift. Your AI agent handles the catalog browsing and order placement for you.

### Who is this for?

- **HR & People Teams** — automate work anniversaries and birthday gifts by asking the AI to send specific items to employees
- **Sales & Customer Success** — send thank-you gifts to clients directly after a successful call without leaving your workflow
- **Marketing Teams** — manage large-scale gifting campaigns for events or product launches through natural language


## Available Tools
- **create_order_batch**: Send a gift to one or more recipients
- **get_campaign**: Get details for a specific campaign
- **get_order_batch**: Get details for a specific order batch
- **get_order**: Get details for a specific order
- **get_product**: Get details for a specific product
- **list_campaigns**: List gifting campaigns
- **list_inventory**: List available inventory for corporate gifts
- **list_order_batches**: List gift order batches
- **list_orders**: List individual gift orders
- **list_products**: List available gifts in Goody
- **list_recipients**: List gift recipients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Goody** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the top 5 gift options under $50."

**🤖 AI Agent:**
> Searching the catalog... Here are 5 popular options under $50: 1. Gourmet Coffee Sampler ($35), 2. Succulent Trio ($42), 3. Artisanal Chocolate Box ($28), 4. Reusable Water Bottle ($30), 5. Wellness Candle ($25). Would you like the product IDs for any of these?

---

**👤 You:**
> "Send a 'Succulent Trio' to John Doe (john@example.com) for his 1-year work anniversary."

**🤖 AI Agent:**
> Creating gift order... I've initiated a gift batch for John Doe. A 'Succulent Trio' gift link will be sent to his email shortly. The order batch ID is BATCH-93021.

---

**👤 You:**
> "Show me the current status of all gifts sent in the last 7 days."

**🤖 AI Agent:**
> Checking recent orders... You sent 3 gifts last week. 'Artisanal Chocolate Box' to Sarah P. was delivered yesterday. 'Wellness Candle' to Mike R. is currently 'Shipped' (ETA tomorrow). 'Succulent Trio' to Jane D. is 'Pending Acceptance'.


## Installation & Usage

To install and use the **Goody** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/goody](https://vinkius.com/mcp/goody)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
