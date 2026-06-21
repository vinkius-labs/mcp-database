# Google Play Developer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-play-developer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-play-developer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-play-developer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Android apps - respond to reviews and check subscriptions via AI.

## Description
Connect your **Google Play Developer** account to your AI agent and streamline your Android app management. Use natural language to monitor user reviews, manage subscriptions, and verify in-app purchases directly from your workflow.

### What you can do

- **Review Management** — Fetch recent reviews, read specific feedback, and post replies directly from the chat
- **Subscription Tracking** — Check the status of user subscriptions, issue refunds, or defer billing dates effortlessly
- **In-App Purchases** — Verify, acknowledge, and consume in-app product purchases
- **Product Catalog** — List all available in-app products and retrieve specific SKU details

### How it works

1. Subscribe to this server
2. Enter your Google Play App Package Name (e.g. com.example.app)
3. Complete the secure Google OAuth flow with a user that has developer access
4. Start managing your app from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **App Developers** — quickly acknowledge test purchases or verify subscription states during development
- **Customer Support** — easily look up a user's subscription or purchase status and issue refunds without opening the Play Console
- **Community Managers** — draft and post professional replies to Google Play reviews directly through the AI agent


## Available Tools
- **acknowledge_product_purchase**: Acknowledge a product purchase
- **cancel_subscription**: Cancel a user subscription
- **consume_product_purchase**: Consume a product purchase
- **defer_subscription**: Defer a subscription billing date
- **get_inapp_product**: Get details for a specific in-app product
- **get_product_purchase**: Check an in-app product purchase status
- **get_review**: Get a specific review by ID
- **get_subscription_purchase**: Check the status of a subscription purchase
- **list_inapp_products**: List in-app products for the app
- **list_reviews**: List recent user reviews for the app
- **refund_subscription**: Refund a subscription
- **reply_to_review**: Reply to a user review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Play Developer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the 5 most recent reviews for our app."

**🤖 AI Agent:**
> Fetching reviews... You have 5 recent reviews. 3 are 5-star reviews praising the new UI. 1 is a 2-star review mentioning a login bug. Would you like me to draft a reply to the 2-star review?

---

**👤 You:**
> "Check the status of subscription token 'abc123xyz' for SKU 'pro_monthly'."

**🤖 AI Agent:**
> Checking subscription... The subscription 'pro_monthly' for this token is currently ACTIVE. The next billing date is scheduled for October 15th.

---

**👤 You:**
> "Refund the subscription linked to token 'refund789' immediately."

**🤖 AI Agent:**
> Processing refund dynamically...
Success. The subscription connected to the provided token has been formally refunded via Google Play services directly.


## Installation & Usage

To install and use the **Google Play Developer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-play-developer](https://vinkius.com/mcp/google-play-developer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
