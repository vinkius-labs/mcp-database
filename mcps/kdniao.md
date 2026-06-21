# KDniao MCP Server

Major logistics tracking platform in China — manage express deliveries, waybills, and status updates via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kdniao)

## Overview
**Category:** ecommerce
**Tools Count:** 8

## Description
Empower your AI agent to orchestrate your logistics and e-commerce operations with **KDniao** (快递鸟), one of the most reliable logistics tracking APIs in China. By connecting KDniao to your agent, you transform complex shipment monitoring, digital waybill management, and delivery forecasting into a natural conversation. Your agent can instantly track packages across hundreds of carriers, identify shippers from tracking numbers, subscribe to status updates, and even estimate arrival times without you ever needing to navigate the comprehensive KDniao portal. Whether you are conducting a supply chain audit or providing real-time customer support for order deliveries, your agent acts as a professional logistics assistant, keeping your data accurate and your operations efficient.

### What you can do

- **Comprehensive Tracking** — Retrieve real-time status and historical traces for any supported domestic or international package.
- **Shipper Identification** — Automatically identify the most likely shipper company for a given tracking number.
- **Update Subscriptions** — Set up automated push notifications to receive real-time alerts when a package status changes.
- **Logistic Estimations** — Retrieve shipping price estimates and predicted arrival times for specific routes.
- **Verification Support** — Identify carriers that require additional recipient verification (like phone number digits).

### How it works

1. Subscribe to this server
2. Enter your KDniao EBusinessID and AppKey
3. Start managing your logistics operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Sellers** — automate tracking updates for customers and audit fulfillment performance through natural language.
- **Supply Chain Teams** — monitor material deliveries and coordinate logistics directly from your AI-powered workspace.
- **Customer Service Leads** — retrieve instant shipment traces to resolve delivery inquiries via a unified AI interface.
- **KDniao Power Users** — integrate your existing logistics workflows into your AI-driven daily routines.


## Available Tools
- **create_electronic_waybill**: Sender/Receiver must be JSON with Name, Mobile, ProvinceName, CityName, ExpAreaName, Address. Uses RequestType 1007.

Create an electronic shipping waybill
- **get_estimated_arrival**: Uses RequestType 8001.

Get estimated delivery time
- **identify_carrier**: Uses RequestType 2002.

Auto-detect carrier from tracking number
- **onsite_pickup**: Uses RequestType 1801.

Request on-site courier pickup
- **preorder_pickup**: Uses RequestType 1001.

Schedule a courier pickup
- **query_shipping_price**: Uses RequestType 1003.

Get shipping price estimate
- **subscribe_tracking**: Uses RequestType 1008.

Subscribe to tracking updates via webhook
- **track_package**: Uses RequestType 1002.

Track a package in real-time


## Installation & Usage

To install and use the **KDniao** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kdniao](https://vinkius.com/mcp/kdniao)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
