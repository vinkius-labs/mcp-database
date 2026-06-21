# WooCommerce Order Status Reader MCP Server

This MCP gives your AI agent the ability to check the real-time status and tracking information of any WooCommerce order using an Order ID or a Customer Email. Perfect for automating "where is my order?" (WISMO) support queries.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/woocommerce-order-status-reader)

## Overview
**Category:** ecommerce
**Tools Count:** 1

## Description
Empower your AI customer support bots to instantly answer the most common e-commerce question: "Where is my order?". This MCP provides a highly restricted, read-only bridge to your WooCommerce store.

### The Superpowers

- **Instant WISMO Resolution:** The AI can look up an order by its exact ID, or search for the most recent orders using just the customer's email address.
- **Zero-Trust Safety:** This is a strictly read-only tool. The agent cannot modify the order, cannot issue refunds, and cannot read orders belonging to other customers unless explicitly asked for that email.
- **Tracking Extraction:** It automatically parses WooCommerce's `_tracking_number` meta data so the AI can provide tracking links and shipping method details directly to the customer.


## Available Tools
- **read_woocommerce_order**: You must provide either the specific orderId or the customer's email address to search for recent orders.

Reads the real-time status of a WooCommerce order


## Installation & Usage

To install and use the **WooCommerce Order Status Reader** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/woocommerce-order-status-reader](https://vinkius.com/mcp/woocommerce-order-status-reader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
