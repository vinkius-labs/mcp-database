# KDniao MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kdniao)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kdniao-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kdniao-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Major logistics tracking platform in China — manage express deliveries, waybills, and status updates via AI.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KDniao** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track package 'YTO123456789' using carrier code 'YTO'."

**🤖 AI Agent:**
> I've retrieved the traces for your YuanTong package. It has been delivered and signed for at 2:30 PM today in Beijing. Would you like to see the full delivery history?

---

**👤 You:**
> "Identify the shipper for tracking number '7890123456'."

**🤖 AI Agent:**
> Based on the tracking number format, the most likely shipper is 'ZTO Express' (ZTO). I can also check if it might belong to other carriers like Yunda or EMS if you prefer.

---

**👤 You:**
> "Estimate arrival time for an SF Express package from Shanghai to Hangzhou."

**🤖 AI Agent:**
> I've checked the route statistics. A standard SF Express shipment from Shanghai to Hangzhou typically arrives within 24 hours. Would you like me to check the estimated price for this route as well?


## Installation & Usage

To install and use the **KDniao** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kdniao](https://vinkius.com/mcp/kdniao)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
