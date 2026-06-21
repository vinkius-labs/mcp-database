# Marketplacer (Enterprise Marketplace Platform) MCP Server

Manage your enterprise marketplace via Marketplacer — list products, track orders, and audit seller networks.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/marketplacer-enterprise-marketplace-platform)

## Overview
**Category:** ecommerce
**Tools Count:** 9

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


## Installation & Usage

To install and use the **Marketplacer (Enterprise Marketplace Platform)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marketplacer-enterprise-marketplace-platform](https://vinkius.com/mcp/marketplacer-enterprise-marketplace-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
