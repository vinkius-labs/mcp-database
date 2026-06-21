# Postscript MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/postscript)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/postscript-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/postscript-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Drive Shopify revenue with SMS and MMS marketing that feels personal, converts browsers into buyers, and builds lasting loyalty.

## Description
Connect your **Postscript** account to any AI agent and take full control of your SMS marketing orchestration through natural conversation. Postscript is the leading SMS platform for Shopify stores, and this integration allows you to retrieve subscriber metadata, monitor campaign performance, and manage automated keywords directly from your chat interface.

### What you can do

- **Subscriber & Audience Orchestration** — List all managed SMS subscribers and retrieve detailed profile metadata programmatically to ensure your outreach is always synchronized.
- **Campaign & Flow Intelligence** — Access and monitor your SMS campaigns and automated flows (like abandoned cart recovery) directly from the AI interface to track engagement metrics.
- **Keyword & Opt-in Control** — List and search through your mobile keywords to maintain a clear overview of your subscription sources via natural language.
- **Operational Monitoring** — Track system responses and manage webhook metadata using simple AI commands.
- **Account Visibility** — Access high-level account and plan metadata to ensure your SMS operations are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Postscript Private API Key from your account settings
3. Start managing your SMS automation from Claude, Cursor, or any MCP-compatible client

No more manual dashboard checking for subscriber status. Your AI acts as a dedicated SMS marketing coordinator or growth manager.

### Who is this for?

- **Shopify Store Owners** — quickly retrieve subscriber summaries and monitor campaign reach without switching apps.
- **E-commerce Marketers** — automate the discovery of top-performing keywords and track automated flows via natural conversation.
- **Operations Teams** — streamline the retrieval of SMS metadata and monitor organizational growth health directly within the chat.


## Available Tools
- **create_subscriber**: Note: Compliance rules apply.

Subscribe a new user
- **create_webhook**: Create a new webhook
- **delete_webhook**: Delete a webhook
- **get_account_info**: Get account details
- **get_campaign**: Get campaign details
- **get_subscriber**: Get subscriber details
- **list_automations**: g., Abandoned Cart).

List SMS automations
- **list_campaigns**: List SMS campaigns
- **list_keywords**: List SMS keywords
- **list_subscribers**: List all SMS subscribers
- **list_webhooks**: List active webhooks
- **update_subscriber**: Update subscriber info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postscript** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active SMS subscribers in Postscript."

**🤖 AI Agent:**
> I've retrieved your subscribers. You have 1,500 active contacts. Notable recent additions include 'Alice Miller' and 'Sarah Chen'. Would you like to see the opt-in source for any of them?

---

**👤 You:**
> "Show me the performance of all active SMS campaigns with conversion rates and revenue attribution."

**🤖 AI Agent:**
> 5 active SMS campaigns this month. "Flash Sale Friday" generated $34,200 from 12,400 messages (2.8% conversion, $2.76 revenue per message). "Abandoned Cart Recovery" recovered $18,700 across 3,400 sends (8.2% conversion). "Welcome Series" onboarded 890 new subscribers with 94% opt-in retention. "VIP Early Access" drove $12,100 from just 800 sends (highest RPM at $15.13). Total SMS revenue: $72,400. Overall unsubscribe rate: 0.4%.

---

**👤 You:**
> "Create a new SMS campaign targeting customers who purchased in the last 30 days but have not reordered."

**🤖 AI Agent:**
> Campaign "Re-order Reminder" created. Audience: 2,340 customers (purchased 30+ days ago, no repeat order). Message: "Missing your favorites? Come back and enjoy 15% off your next order with code RETURN15. Shop now: [link]". Scheduled: Tomorrow at 11 AM EST (optimal send time). Estimated reach: 2,280 deliverable. Projected revenue based on similar campaigns: $4,600-$6,200.


## Installation & Usage

To install and use the **Postscript** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postscript](https://vinkius.com/mcp/postscript)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
