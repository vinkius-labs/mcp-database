# Nue.io Revenue MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nueio-revenue)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nueio-revenue-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nueio-revenue-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage the revenue lifecycle via Nue.io — track product catalogs, price tags, and revenue workflows directly from your AI agent.

## Description
Connect your **Nue.io** account to your AI agent and streamline your quote-to-revenue operations through natural conversation.

### What you can do

- **Catalog Management** — List all published products, services, and bundles available for self-service.
- **Pricing Intelligence** — Access detailed price tags (Quantity, Tiered, Volume) and pricing logic for specific products.
- **Metadata Mapping** — List business objects available for Stripe metadata mapping and integration.
- **Workflow Tracking** — Monitor automated revenue workflows for billing, collections, and quote processing.
- **Integration Oversight** — View all active third-party integrations (Stripe, Salesforce) connected to your account.
- **Deep Inspection** — Fetch complete metadata and configuration for specific products or bundles using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Nue.io API Key
3. Start managing your revenue catalog from Claude, Cursor, or any MCP client

### Who is this for?

- **Revenue Operations** — quickly check product configurations or price tag logic without opening the dashboard.
- **Sales Teams** — verify available bundles and self-service product details during the quoting process.
- **Finance Managers** — automate the retrieval of revenue workflow data and integration statuses.


## Available Tools
- **get_current_user**: Get current user metadata
- **get_organization_info**: Get organization metadata
- **get_product_details**: Get specific product metadata
- **list_product_bundles**: List configured product bundles
- **list_product_categories**: List catalog categories
- **list_active_integrations**: g., Stripe, Salesforce) connected to Nue.

List connected third-party integrations
- **list_product_price_tags**: List price tags for a product
- **list_catalog_products**: List all published products
- **list_metadata_source_objects**: List objects for metadata mapping
- **list_revenue_workflows**: List automated revenue workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nue.io Revenue** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the products currently published in my Nue.io catalog."

**🤖 AI Agent:**
> Retrieving your catalog... I found 12 published products, including 'Enterprise SaaS Bundle', 'API Access Pack', and 'Premium Support'. Would you like to see the pricing logic for the Enterprise SaaS Bundle?

---

**👤 You:**
> "What are the price tags associated with product ID 'prod_98765'?"

**🤖 AI Agent:**
> Fetching price tags for prod_98765... This product has 2 price tags: 'Volume Tiered' (Standard) and 'Annual Commitment' (Discounted). Shall I provide the specific price per unit for each volume range?

---

**👤 You:**
> "Show me our active revenue and billing workflows."

**🤖 AI Agent:**
> Retrieving revenue workflows... You have 3 active workflows: 'Automated Invoice Generation', 'Credit Memo Approval', and 'Renewal Reminder Path'. Would you like the configuration details for the invoice generation workflow?


## Installation & Usage

To install and use the **Nue.io Revenue** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nueio-revenue](https://vinkius.com/mcp/nueio-revenue)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
