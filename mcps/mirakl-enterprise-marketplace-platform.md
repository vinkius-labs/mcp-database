# Mirakl (Enterprise Marketplace Platform) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mirakl-enterprise-marketplace-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mirakl-enterprise-marketplace-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mirakl-enterprise-marketplace-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your enterprise marketplace via Mirakl — list global offers, track multi-vendor orders, and audit seller shops.

## Description
Connect your **Mirakl** instance to any AI agent and take full control of your enterprise marketplace operations, seller network, and global offer management through natural conversation.

### What you can do

- **Offer Orchestration** — List and retrieve detailed marketplace offers from multiple sellers, including inventory availability and specific pricing constraints directly from your agent
- **Order Monitoring** — Track multi-vendor checkout transactions and retrieve full line-item details, payment statuses, and fulfillment histories securely
- **Seller Management** — Enumerate third-party shops (sellers) active on your platform and retrieve detailed compliance profiles and operational configurations natively
- **Catalog & Category Audit** — Explore the broad platform product catalog and navigate hierarchical category trees to understand your marketplace's structural taxonomy
- **Financial Visibility** — List and audit structural accounting invoices and settlements triggered against seller shops to manage your marketplace's financial boundaries
- **Communication Stream** — Retrieve threaded messages between buyers, sellers, and operators to monitor support logs and platform interactions efficiently
- **Metadata Inspection** — Deep-dive into specific Offer or Order IDs to retrieve precise JSON representations and chronological transaction insights instantly

### How it works

1. Subscribe to this server
2. Enter your Mirakl Environment URL and API Key
3. Start managing your marketplace platform from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketplace Operators** — monitor multi-vendor order flows and seller performance through natural conversation without manual portal navigation
- **E-commerce Leads** — audit global offer distributions and category taxonomies directly from your workspace to optimize product discovery
- **Finance & Compliance Teams** — track marketplace invoices and seller compliance profiles efficiently to maintain high platform standards


## Available Tools
- **list_offers**: Represents the exact live inventory binding a specific product to a specific explicit price from a Shop.

List global Marketplace offers created by multiple sellers
- **get_offer**: Get an explicit Mirakl offer entity mapping seller limits
- **list_orders**: List Mirakl marketplace multi-vendor checkout orders
- **get_order**: Get deep details tracing a specific Marketplace Order transaction
- **list_shops**: List third-party Seller accounts (Shops) operating
- **get_shop**: Get deep configurations tracking an explicit Mirakl Seller Shop
- **list_products**: List broad Platform Product Catalog nodes
- **list_categories**: g. Electronics -> Computers).

List static structural Mirakl marketplace Category Trees
- **list_messages**: List internal Marketplace communication messages
- **list_invoices**: List explicit Mirakl structural accounting invoices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mirakl (Enterprise Marketplace Platform)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active seller shops in my Mirakl marketplace"

**🤖 AI Agent:**
> I've retrieved your list of active shops. Highlights include 'Tech World' (ID: shop-123), 'Home & Garden Pro' (ID: shop-456), and 'Direct Sport' (ID: shop-789). Would you like to see the compliance status or offer count for any of these?

---

**👤 You:**
> "Show me the last 5 invoices generated for seller shops"

**🤖 AI Agent:**
> Retrieving latest invoices… I've identified 5 recent settlements. Highlights: Invoice #INV-1001 (€1,250 for Shop A), Invoice #INV-1002 (€850 for Shop B), and Invoice #INV-1003 (€45.50). Would you like to see the settlement details for the largest invoice?

---

**👤 You:**
> "Search for messages related to order ID 'order-987'"

**🤖 AI Agent:**
> Searching communication history… I've found a thread for order 'order-987' between the buyer and the seller. The customer is asking about the delivery timeframe. Would you like me to retrieve the full message content or draft a reply as the operator?


## Installation & Usage

To install and use the **Mirakl (Enterprise Marketplace Platform)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mirakl-enterprise-marketplace-platform](https://vinkius.com/mcp/mirakl-enterprise-marketplace-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
