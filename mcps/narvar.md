# Narvar MCP Server

Streamline post-purchase experiences — track shipments, manage returns, and provide delivery estimates directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/narvar)

## Overview
**Category:** ecommerce
**Tools Count:** 5

## Description
Connect **Narvar** to your AI agent to take full control of the post-purchase customer journey. From real-time tracking to automated returns, manage every logistics touchpoint through natural conversation.

### What you can do

- **Shipment Tracking** — Get real-time status updates and event history for any carrier tracking number using `get_tracking`.
- **Returns Management** — Initiate return requests and generate labels for orders instantly with `create_return`.
- **Order Insights** — Retrieve comprehensive order details, line items, and fulfillment status using `get_order`.
- **Customer Notifications** — Trigger transactional Email or SMS notifications for shipment milestones with `trigger_notification`.
- **Delivery Estimates** — Calculate precise estimated delivery dates (EDD) for checkout optimization using `get_estimated_delivery_dates`.

### How it works

1. Subscribe to this server
2. Enter your Narvar API Key
3. Start managing logistics from Claude, Cursor, or any MCP-compatible client

No more switching between carrier portals and internal dashboards. Your AI acts as a dedicated logistics coordinator.

### Who is this for?

- **E-commerce Managers** — Monitor shipment health and order fulfillment across multiple carriers in one view.
- **Customer Support Teams** — Instantly answer "where is my order" queries and process returns without leaving the chat.
- **Logistics Operations** — Analyze delivery performance and trigger customer alerts for delays or successful deliveries.


## Available Tools
- **get_estimated_delivery_dates**: Uses POST but acts as a query.

Calculate estimated delivery dates (EDD)
- **create_return**: Initiate a return request for an order
- **trigger_notification**: Trigger a transactional notification
- **get_order**: Get comprehensive order details
- **get_tracking**: Get real-time tracking information for a shipment


## Installation & Usage

To install and use the **Narvar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/narvar](https://vinkius.com/mcp/narvar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
