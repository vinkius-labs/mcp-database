# Payhip MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/payhip)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/payhip-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/payhip-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Sell ebooks, courses, memberships, and digital downloads directly to your audience with zero upfront costs and simple setup.

## Description
Connect your **Payhip** account to any AI agent and take full control of your digital product orchestration through natural conversation. Payhip is a powerful platform for selling downloads and software, and this integration allows you to manage discount coupons, verify customer license keys, and track software usage directly from your chat interface.

### What you can do

- **Coupon & Promotion Orchestration** — List and manage discount coupons programmatically to ensure your marketing campaigns are always synchronized.
- **License Key Intelligence** — Verify software license keys in real-time and retrieve detailed validation metadata directly from the AI interface to prevent piracy.
- **Compliance & License Control** — Enable or disable specific license keys via natural language to maintain a clear overview of your customer entitlements.
- **Usage Monitoring Oversight** — Track and update license usage counts (increments or decrements) using simple AI commands to ensure your software terms are always enforced.
- **Operational Monitoring** — Track system responses and manage developer metadata to ensure your digital storefront is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Payhip API Key from your developer settings
3. Start managing your store's licensing and coupons from Claude, Cursor, or any MCP-compatible client

No more manual license checking or spreadsheet coupon tracking. Your AI acts as a dedicated digital operations manager or license coordinator.

### Who is this for?

- **Software Developers & Founders** — quickly verify customer licenses and monitor usage without switching apps.
- **Digital Creators** — automate the creation of promotional codes and track campaign reach via natural conversation.
- **Support Teams** — streamline the retrieval of license metadata and monitor organizational health directly within the chat.


## Available Tools
- **create_coupon**: Requires code, discount type, and amount.

Create a new coupon
- **disable_license**: g., after refund).

Disable a license key
- **enable_license**: Enable a license key
- **get_coupon**: Get details for a specific coupon
- **get_customer_details**: Get details for a specific customer
- **get_product_details**: Get details for a specific product
- **list_coupons**: List all Payhip coupons
- **list_customers**: List all store customers
- **list_products**: List all digital products
- **update_license_usage**: Update license usage count
- **verify_license**: Verify a software license key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Payhip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify license key 'ABCD-1234' for product link 'https://payhip.com/b/xyz'."

**🤖 AI Agent:**
> I've verified the license. It is currently 'Active' for customer 'John Doe' (ID: 991). Would you like me to increase the usage count for this key?

---

**👤 You:**
> "Show me all active coupons and their usage statistics for my Payhip store."

**🤖 AI Agent:**
> You have 6 active coupons. "SUMMER30" (30% off) has been used 47 times generating $2,340 in discounted sales. "LAUNCH50" (50% off) was used 23 times. "WELCOME15" is your most popular at 89 redemptions. 2 coupons expire within 7 days. Total discount value given this month: $1,847.

---

**👤 You:**
> "Verify the license key LK-8847-ABCD for my premium plugin product and check its usage count."

**🤖 AI Agent:**
> License LK-8847-ABCD is valid and active. Product: Premium Plugin Suite. Purchased by: tech@meridian.io on March 15, 2025. Current usage: 3 of 5 allowed activations. Last activation: May 2nd from IP 192.168.1.45. The license is set to renew annually on March 15, 2026.


## Installation & Usage

To install and use the **Payhip** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/payhip](https://vinkius.com/mcp/payhip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
