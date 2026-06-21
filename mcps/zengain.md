# Zengain MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zengain)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zengain-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zengain-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Identify high-intent website visitors by company and reach out to warm leads before they fill out a form or contact you.

## Description
Connect your **Zengain** (Nalpeiron Growth Platform) account to any AI agent and simplify your customer success and usage analytics workflows through natural conversation.

### What you can do

- **Product Lifecycle** — List all registered products and retrieve detailed configuration metadata
- **User Engagement** — Query product users, inspect their profiles, and calculate real-time health scores
- **Usage Analytics** — Get high-level analytics summaries and track custom events to monitor feature adoption
- **KPM Tracking** — Monitor Key Product Milestones to identify successful onboarding and churn risks
- **System Monitoring** — List configured webhooks to understand your integration data flow

### How it works

1. Subscribe to this server
2. Enter your Zengain Tenant ID and API Key
3. Start managing your customer success resources from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_health_score**: Get customer health score
- **get_product**: Get details for a specific product
- **get_analytics_summary**: Get analytics summary
- **get_user_details**: Get details for a specific user
- **list_events**: List tracking events
- **list_kpms**: List Key Product Milestones
- **list_products**: List Zengain products
- **list_users**: List product users
- **list_webhooks**: List configured webhooks
- **track_event**: Track a custom event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zengain** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Zengain account."

**🤖 AI Agent:**
> I've found 3 products: 'Desktop App v2', 'Cloud SaaS Portal', and 'Mobile Lite'. Which one should I analyze?

---

**👤 You:**
> "What is the health score for user 'customer_456'?"

**🤖 AI Agent:**
> User 'customer_456' has a health score of 82/100 (Good). Their engagement has increased by 15% over the last 30 days.

---

**👤 You:**
> "Show me a summary of usage analytics for this month."

**🤖 AI Agent:**
> Across all products, you have 1,200 Daily Active Users (DAU) and 5,500 Monthly Active Users (MAU). Feature adoption for 'Real-time Sync' is at an all-time high.


## Installation & Usage

To install and use the **Zengain** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zengain](https://vinkius.com/mcp/zengain)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
