# Refersion MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/refersion)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/refersion-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/refersion-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your affiliate marketing program via Refersion — list affiliates, track conversions, and manage webhooks directly from any AI agent.

## Description
Connect your **Refersion** account to any AI agent to streamline your affiliate marketing operations through natural conversation.

### What you can do

- **Affiliate Management** — List all registered affiliates, fetch detailed profiles using unique IDs, and register new affiliate accounts instantly.
- **Conversion Tracking** — Query all recorded conversions and create new conversion records to credit your partners accurately for sales.
- **Real-time Updates** — List existing webhook configurations and register new listeners to receive real-time updates on program activities.
- **Deep Inspection** — Fetch complete metadata for specific affiliates and conversions to resolve disputes or analyze performance.

### How it works

1. Subscribe to this server
2. Enter your Refersion Public Key and Secret Key
3. Start managing your affiliate network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Affiliate Managers** — quickly check affiliate details and approve conversions without digging through the dashboard
- **Marketing Teams** — automate the retrieval of performance data and affiliate lists for reporting
- **Developers** — test and manage webhooks and conversion logic directly from the coding environment


## Available Tools
- **create_affiliate**: Create a new affiliate
- **create_conversion**: Create a new conversion
- **create_webhook**: Registers a new webhook listener
- **get_affiliate**: Get details for a specific affiliate
- **get_conversion**: Get details for a specific conversion
- **list_affiliates**: List affiliates for your account
- **list_conversions**: List conversions
- **list_webhooks**: List configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refersion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current affiliates in Refersion."

**🤖 AI Agent:**
> I've retrieved your affiliate list. You have 12 active affiliates, including 'Sarah Jenkins' (ID: aff_882) and 'Tech Reviews Inc' (ID: aff_901). Would you like details on a specific one?

---

**👤 You:**
> "Create a new conversion of 75.00 USD for affiliate ID aff_882."

**🤖 AI Agent:**
> The conversion has been successfully recorded. A new entry for $75.00 USD has been credited to affiliate aff_882 (Sarah Jenkins).

---

**👤 You:**
> "Show me all configured webhooks."

**🤖 AI Agent:**
> You currently have 2 webhooks configured: one for 'New Affiliate' events pointing to your production server and another for 'New Conversion' events.


## Installation & Usage

To install and use the **Refersion** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/refersion](https://vinkius.com/mcp/refersion)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
