# Marketplacer (Enterprise Marketplace Platform) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marketplacer-enterprise-marketplace-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/marketplacer-enterprise-marketplace-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/marketplacer-enterprise-marketplace-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your enterprise marketplace via Marketplacer — list products, track orders, and audit seller networks.

## Description
Connect your **Marketplacer** instance to any AI agent and take full control of your enterprise marketplace operations, seller network, and product catalog through natural conversation.

### What you can do

- **Product Orchestration** — List and retrieve detailed product metadata (adverts) including pricing, variants, and descriptions using GraphQL-based node identifiers directly from your agent
- **Order & Invoice Audit** — Track marketplace orders by listing recent invoices and extracting detailed payloads reflecting line items, tax distributions, and customer data
- **Seller Management** — Enumerate third-party sellers and vendors active on your platform to audit vendor listings and account statuses securely
- **Taxonomy Navigation** — Explore complex category trees and product hierarchies to understand your marketplace's architectural taxonomy and item distributions
- **Logistics Monitoring** — List and inspect shipment records to track the fulfillment lifecycle of orders across your distributed seller network
- **Webhooks & Events** — Audit configured event subscriptions and webhooks to ensure your marketplace's automated integrations are functioning correctly
- **Advanced Custom Queries** — Execute ad-hoc sophisticated GraphQL queries using native syntax to fetch literal data points across any schema entity

### How it works

1. Subscribe to this server
2. Enter your Marketplacer API URL and API Key
3. Start managing your marketplace infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketplace Managers** — monitor order flows and vendor performance through natural conversation without manual report generation
- **Software Developers** — test GraphQL queries and verify product attribute mappings directly from your workspace terminal
- **Dropshipping Operations** — audit shipment statuses and track cross-vendor invoices efficiently to maintain high fulfillment standards


## Available Tools
- **list_adverts**: Use this tool to list product items.

List Marketplacer adverts (products)
- **get_advert**: Get Marketplacer advert by node ID
- **list_invoices**: Use this to track all registered orders on the platform.

List Marketplacer invoices (orders)
- **get_invoice**: Get Marketplacer invoice by node ID
- **list_sellers**: Use to fetch vendor lists.

List Marketplacer sellers/vendors
- **list_categories**: List Marketplacer category taxonomies
- **list_webhooks**: List Marketplacer webhooks (events subscription)
- **list_shipments**: List Marketplacer shipments
- **graphql_query**: Run standard GraphQL queries against Marketplacer endpoint


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marketplacer (Enterprise Marketplace Platform)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 invoices in my Marketplacer instance"

**🤖 AI Agent:**
> I've retrieved the latest 5 invoices. Highlights include Invoice #INV-123 ($150.00 from Seller A) and Invoice #INV-456 ($85.50 from Seller B). Would you like to see the shipment status for any of these?

---

**👤 You:**
> "Search for sellers containing 'Outdoor' in the network"

**🤖 AI Agent:**
> Searching seller network… I've identified 3 vendors: 'Outdoor Adventure Gear' (ID: sel-123), 'Premium Outdoor Living' (ID: sel-456), and 'The Great Outdoors' (ID: sel-789). I can fetch the advert count for each seller if you'd like.

---

**👤 You:**
> "Run a GraphQL query to fetch the 'legacyId' and 'title' for advert ID 'node-987'"

**🤖 AI Agent:**
> Executing custom query… Done. For advert 'node-987', the Legacy ID is '554433' and the Title is 'Titanium Mountain Bike'. Would you like to fetch the inventory quantity using another query?


## Installation & Usage

To install and use the **Marketplacer (Enterprise Marketplace Platform)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marketplacer-enterprise-marketplace-platform](https://vinkius.com/mcp/marketplacer-enterprise-marketplace-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
