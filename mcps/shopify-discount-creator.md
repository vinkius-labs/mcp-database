# Shopify Discount Creator MCP Server

This MCP does exactly one thing: it creates unique percentage discount codes in your Shopify store on the fly. Incredible for giving your AI agent the power to prevent cart abandonment during a chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/shopify-discount-creator)

## Overview
**Category:** industry-titans
**Tools Count:** 1

## Description
We refused to build a bloated Shopify integration that requires reading your entire product catalog, modifying inventory, and accessing your customer's personal data. Instead, this MCP server provides a surgical, zero-trust bridge: **just creating discount codes.**

Your AI agent gains the immediate ability to act as a real-time sales closer. If a customer is hesitating in the chat because of the price, the agent doesn't need to ask for human approval—it instantly generates a unique 10% off code and drops it in the chat to secure the sale.

### The Superpowers

- **Real-Time Closing:** End cart abandonment friction. The AI can sense hesitation and automatically generate a custom discount code (e.g., `VIP_SAVE_15`) exactly when needed.
- **Zero-Bloat Integration:** No massive Shopify SDKs. It uses a direct `POST` to the Shopify Admin REST API. You only need a Custom App token with `write_discounts` permission.
- **Absolute Containment:** Because this is strictly a "Push-only" creation tool scoped only to discounts, the agent cannot read your orders, cannot delete products, and cannot access customer data. It only generates codes. A completely secure, one-way funnel.


## Available Tools
- **create_shopify_discount**: Provide the desired code name (e.g. VIP_10) and the percentage amount to discount (e.g. 10 for 10% off). Send the resulting code directly to the customer.

Generates a new percentage-based discount code in Shopify on the fly


## Installation & Usage

To install and use the **Shopify Discount Creator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shopify-discount-creator](https://vinkius.com/mcp/shopify-discount-creator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
