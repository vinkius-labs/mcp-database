# Gumroad MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gumroad-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gumroad-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gumroad-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Sell digital products, memberships, and physical goods directly to your audience with a checkout that handles everything.

## Description
Connect your **Gumroad** account to any AI agent and take full control of your digital products and e-commerce workflows through natural conversation.

### What you can do

- **Product Management** — List all your digital products and retrieve detailed metadata, pricing, and shareable URLs programmatically
- **Sales Intelligence** — Monitor transaction history with precise date filters to track revenue and customer acquisition trends
- **Offer Code Automation** — Create and manage discount codes (fixed or percentage-based) to drive marketing campaigns and sales
- **Customer Relationships** — List and manage product-specific subscribers to maintain direct communication with your audience
- **Store Performance** — Retrieve complete transaction details for any sale ID to provide high-fidelity customer support

### How it works

1. Subscribe to this server
2. Retrieve your Application Token from your Gumroad Dashboard (Settings > Advanced > Application tokens)
3. Start managing your creator business from Claude, Cursor, or any MCP client

No more manual status checking or complex store management through different tabs. Your AI acts as your dedicated store manager.

### Who is this for?

- **Digital Creators** — automate discount code generation and monitor sales performance through natural language
- **Customer Success Managers** — quickly retrieve customer transaction data to verify purchases and handle support requests
- **Growth Marketers** — track subscriber lists and campaign performance across multiple products without leaving your workspace


## Available Tools
- **create_offer_code**: Create a new discount code
- **get_product_details**: Get details for a product
- **get_sale_details**: Get details for a specific sale
- **get_user_profile**: Get your Gumroad account details
- **list_offer_codes**: List discount codes for a product
- **list_products**: List your Gumroad products
- **list_sales**: Supports date filtering.

List recent sales
- **list_product_subscribers**: List subscribers for a product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gumroad** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my products on Gumroad."

**🤖 AI Agent:**
> I've retrieved your digital products. You have 5 active items, including 'Advanced AI Guide' ($49.00) and 'MCP Templates' ($19.00). Would you like the shareable URLs for any of these?

---

**👤 You:**
> "Show me the sales from the last 7 days."

**🤖 AI Agent:**
> Scanning transaction history... In the last 7 days, you've had 12 sales totaling $345.00. The best-selling product was 'MCP Templates'. Would you like a breakdown of each transaction?

---

**👤 You:**
> "Create a 20% discount code named 'SUMMER26' for my AI Guide product."

**🤖 AI Agent:**
> Done! I've created the offer code 'SUMMER26' for your 'Advanced AI Guide'. It provides a 20% discount and is ready for use on your checkout page.


## Installation & Usage

To install and use the **Gumroad** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gumroad-alternative](https://vinkius.com/mcp/gumroad-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
