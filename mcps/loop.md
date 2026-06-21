# Loop MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loop)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/loop-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/loop-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Collect customer feedback through micro-surveys that measure NPS, CSAT, and product sentiment without disrupting the user experience.

## Description
Connect your **Loop** account to any AI agent and manage returns through natural conversation.

### What you can do

- **Return Tracking** — Browse return requests with status and reason codes
- **Exchange Management** — Track product exchanges and new order creation
- **Refund History** — Monitor refunds with amounts and processing status
- **Return Analytics** — Access return rates, top reasons, and trend data
- **Customer Returns** — View return history per customer

### How it works

1. Subscribe to this server
2. Enter your Loop API Key
3. Start managing returns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Teams** — manage returns and reduce churn
- **Customer Support** — process returns and exchanges efficiently
- **Operations** — analyze return trends and optimize logistics


## Available Tools
- **list_projects**: List projects in Loop
- **list_feedback_sources**: ) providing feedback.

List integrated feedback sources
- **list_feedback_themes**: List recurring feedback themes
- **list_dev_tickets**: List AI-generated developer tickets
- **add_internal_note**: Add an internal note to a feedback item
- **get_feedback_details**: Get details of a specific feedback item
- **get_me**: Get account information
- **get_sentiment_metrics**: Get overall sentiment analytics
- **get_ticket_details**: Get details of a developer ticket
- **list_feedback**: List customer feedback items in Loop


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show return requests from this week and top return reasons."

**🤖 AI Agent:**
> This week: 23 returns. Pending: 8, Approved: 12, Rejected: 3. Exchanges: 6 (26%). Refunds: 14 (61%). Store credit: 3 (13%). Top reasons: 'Wrong size' (9, 39%), 'Not as described' (5, 22%), 'Defective' (4, 17%), 'Changed mind' (3, 13%), 'Late delivery' (2, 9%). Return rate: 4.2%.

---

**👤 You:**
> "Show return analytics and products with highest return rates."

**🤖 AI Agent:**
> Return analytics (30 days): 89 returns, 4.2% rate. Exchange rate: 28% (25 exchanges saved $2,100 in revenue). Top return products: 'Slim Fit Shirt M' (12 returns, 15% rate ⚠️). 'Running Shoes 10' (8, 8%). 'Wireless Headphones' (6, 3%). Refund total: $4,580. Average processing: 2.1 days. Customer retention post-return: 72%.

---

**👤 You:**
> "Show return history for customer sarah@company.com and pending refunds."

**🤖 AI Agent:**
> sarah@company.com: 2 returns (last 6 months). 1) 'Slim Fit Shirt L' — exchanged for XL ✅ (Mar 15). 2) 'Wireless Mouse' — refunded $45 ✅ (Feb 8, defective). Lifetime orders: 12 ($890). Return rate: 17% (above avg ⚠️). Pending refunds (all customers): 5 total, $234. Oldest: 3 days (Sarah, $45). Processing: automatic.


## Installation & Usage

To install and use the **Loop** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loop](https://vinkius.com/mcp/loop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
