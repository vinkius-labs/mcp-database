# WooCommerce Order Status Reader MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/woocommerce-order-status-reader)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/woocommerce-order-status-reader-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/woocommerce-order-status-reader-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

This MCP gives your AI agent the ability to check the real-time status and tracking information of any WooCommerce order using an Order ID or a Customer Email. Perfect for automating "where is my order?" (WISMO) support queries.

## Description
Empower your AI customer support bots to instantly answer the most common e-commerce question: "Where is my order?". This MCP provides a highly restricted, read-only bridge to your WooCommerce store.

### The Superpowers

- **Instant WISMO Resolution:** The AI can look up an order by its exact ID, or search for the most recent orders using just the customer's email address.
- **Zero-Trust Safety:** This is a strictly read-only tool. The agent cannot modify the order, cannot issue refunds, and cannot read orders belonging to other customers unless explicitly asked for that email.
- **Tracking Extraction:** It automatically parses WooCommerce's `_tracking_number` meta data so the AI can provide tracking links and shipping method details directly to the customer.


## Available Tools
- **read_woocommerce_order**: You must provide either the specific orderId or the customer's email address to search for recent orders.

Reads the real-time status of a WooCommerce order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WooCommerce Order Status Reader** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "A customer is asking for the status of order #10452. Can you check it for them?"

**🤖 AI Agent:**
> I've checked the status of Order #10452. It is currently **COMPLETED** and was shipped via FedEx. The tracking number is 1Z9999999999999999.


## Installation & Usage

To install and use the **WooCommerce Order Status Reader** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/woocommerce-order-status-reader](https://vinkius.com/mcp/woocommerce-order-status-reader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
