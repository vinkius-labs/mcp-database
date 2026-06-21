# Vouchery.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/voucheryio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/voucheryio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/voucheryio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage coupon, discount, and loyalty programs on Vouchery.io with AI agents.

## Description
Connect your **Vouchery.io** account to any AI agent to automate your promotional marketing and loyalty workflows. Vouchery provides a powerful infrastructure for creating, distributing, and tracking personalized digital rewards and incentives through natural conversation.

### What you can do

- **Campaign Orchestration** — Create and manage complex marketing campaigns, including discount, referral, and loyalty programs programmatically.
- **Voucher Automation** — Generate unique voucher codes and monitor their status to ensure secure and controlled reward distribution.
- **Redemption Control** — Redeem vouchers and record detailed transaction histories to prevent fraud and track campaign ROI.
- **Customer Insights** — Access and manage customer profiles to track engagement levels and reward usage history.
- **Lifecycle Management** — Securely delete expired campaigns and vouchers to maintain a clean promotional database via natural language.

### How it works

1. Subscribe to this server
2. Enter your Vouchery.io API Key from your dashboard
3. Select your environment mode (Production or Preview/Sandbox)
4. Start managing your promotional rewards from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Marketers** — quickly generate new promo codes and monitor campaign performance without switching tabs.
- **Growth Hackers** — automate referral program management and reward distribution via natural language commands.
- **Loyalty Managers** — track customer engagement and manage personalized rewards efficiently within the AI interface.


## Available Tools
- **create_campaign**: Provide name and type.

Create a new marketing campaign
- **create_customer**: Create or update a customer profile
- **create_voucher**: Generate a new voucher code for a campaign
- **delete_campaign**: Delete a campaign
- **delete_voucher**: Delete a voucher code
- **get_campaign**: Get details of a specific campaign
- **get_customer**: Get details of a customer
- **get_voucher**: Get details of a specific voucher code
- **list_campaigns**: List all marketing campaigns
- **list_customers**: List all customers
- **list_redemptions**: List redemptions for a voucher
- **redeem_voucher**: Redeem (claim) a voucher code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vouchery.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new discount campaign called 'Black Friday VIP 2024' in Vouchery and generate a unique promo code for it."

**🤖 AI Agent:**
> I've successfully created the 'Black Friday VIP 2024' discount campaign. I also generated a unique voucher code for it: 'BF-VIP-8A9F'. The campaign is now live and ready to be assigned to your top-tier customers.

---

**👤 You:**
> "Redeem the voucher code 'WELCOME-20' for customer 'sarah@piedpiper.com' under transaction ID 'TXN-49281'."

**🤖 AI Agent:**
> The voucher 'WELCOME-20' has been successfully redeemed for 'sarah@piedpiper.com'. The transaction 'TXN-49281' has been recorded in the campaign history, and her loyalty profile has been updated.

---

**👤 You:**
> "Show me the redemption history and current status for the promo code 'INFLUENCER-100'."

**🤖 AI Agent:**
> The voucher 'INFLUENCER-100' is currently active. It has been redeemed 42 times so far, with the most recent redemption by 'alex@starkindustries.com' on transaction 'TXN-10293'. It has 58 uses remaining before hitting its limit.


## Installation & Usage

To install and use the **Vouchery.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/voucheryio](https://vinkius.com/mcp/voucheryio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
