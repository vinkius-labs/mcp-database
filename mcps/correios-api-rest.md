# Correios API (REST) MCP Server

Track Brazilian postal objects and calculate shipping prices and deadlines directly through the official Correios REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/correios-api-rest)

## Overview
**Category:** ecommerce
**Tools Count:** 2

## Description
Connect your AI agent to the **Correios** infrastructure to automate logistics queries in Brazil. This server provides direct access to the official REST API for real-time tracking and shipping simulations.

### What you can do

- **Object Tracking** — Get the full history of events and current status for any valid tracking code (e.g., AA123456789BR) using the `track_object` tool.
- **Shipping Calculation** — Simulate prices and delivery deadlines for various services like SEDEX and PAC based on weight, dimensions, and zip codes with `calculate_price_deadline`.
- **Logistics Automation** — Integrate shipping data into your e-commerce or support workflows without manual lookups.

### How it works

1. Subscribe to this server
2. Enter your Correios API credentials (User and Password)
3. Start querying logistics data from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Owners** — quickly check delivery statuses for customers and provide proactive updates.
- **Logistics Managers** — automate shipping cost estimations for different regions in Brazil directly from the terminal or chat.
- **Support Teams** — provide instant tracking updates within AI-powered chat interfaces without leaving the conversation.


## Available Tools
- **calculate_price_deadline**: Uses POST but acts as a query.

Calculate shipping price and deadline
- **track_object**: Track a postal object


## Installation & Usage

To install and use the **Correios API (REST)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/correios-api-rest](https://vinkius.com/mcp/correios-api-rest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
