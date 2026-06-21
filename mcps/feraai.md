# Fera.ai MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feraai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/feraai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/feraai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-experience](../categories/customer-experience.md)

Manage reviews and social proof via Fera.ai — list customer feedback, track product ratings, and monitor UGC directly through your AI agent.

## Description
Connect your **Fera.ai** account to any AI agent and take full control of your customer reviews, ratings, and user-generated content (UGC) through natural conversation.

### What you can do

- **Review Orchestration** — List all customer reviews and fetch detailed sentiment metadata for specific feedback natively
- **Rating Intelligence** — Query aggregated product ratings and review counts to analyze catalog performance flawlessly
- **UGC Monitoring** — List and inspect customer-submitted photos and videos to manage your visual social proof natively
- **Customer Insights** — Access detailed profiles of customers who have submitted feedback to personalize engagement synchronously
- **Multi-Store Management** — List and query data across all stores managed under your partner or business account flawlessly
- **Integration Audit** — Monitor active external integrations with platforms like Shopify, Wix, and BigCommerce directly from the cloud
- **Identity Context** — Verify your API secret key identity and account subscription details through the agent flawlessly

### How it works

1. Subscribe to this server
2. Enter your Fera.ai Private API Secret Key
3. Start managing your social proof from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor new reviews and product ratings without manual dashboard exports
- **Customer Support Teams** — quickly look up specific review details to address customer concerns via chat
- **Marketing Analysts** — pull raw UGC and review data directly into your AI-powered performance workflow


## Available Tools
- **get_account_info**: Get Fera account and subscription details
- **get_customer**: Get details for a specific customer profile
- **get_me**: Get current API token identity info
- **get_product_rating**: Get aggregated rating and review count for a product
- **get_review**: Get details for a specific review
- **list_site_content**: List social proof content and widgets
- **list_customers**: List customers who have submitted feedback
- **list_external_integrations**: List active external integrations (Shopify, etc.)
- **list_media**: List customer-submitted photos and videos (UGC)
- **list_products**: List products being tracked by Fera
- **list_reviews**: List all customer reviews for your store
- **list_stores**: List stores managed under your account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fera.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the latest 5 reviews for my store."

**🤖 AI Agent:**
> I've retrieved your recent reviews. Your store currently has a 4.8 average rating. The latest feedback includes 'Amazing quality!' from Jane and 'Fast shipping' from Mark. Would you like to see the details for any of these?

---

**👤 You:**
> "Show me the average rating for product SKU-123."

**🤖 AI Agent:**
> Fetching ratings for SKU-123... This product has a 4.5 rating based on 42 verified reviews. 85% of customers gave it 5 stars. Shall I retrieve the latest photo reviews for this product?

---

**👤 You:**
> "Check my active integrations on Fera."

**🤖 AI Agent:**
> Inspecting integrations... Your Fera account is currently connected to Shopify (Active) and Klaviyo (Active). You also have the Google Search results integration enabled.


## Installation & Usage

To install and use the **Fera.ai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feraai](https://vinkius.com/mcp/feraai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
