# Memberstack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/memberstack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/memberstack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/memberstack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Member authentication and user management via Memberstack — manage members, plans, and custom fields.

## Description
Connect your **Memberstack** account to any AI agent and take full control of your member management and authentication workflows through natural conversation.

### What you can do

- **Member Administration** — List all members, search by email, and fetch detailed metadata including plan connections
- **Plan Management** — Enumerate membership plans and retrieve detailed configurations for free and paid offerings
- **Custom Data Handling** — List and manage custom fields defined for your members
- **Promotion & Offers** — Access and monitor active coupons and marketing promotions
- **App Visibility** — Retrieve high-level information about your current Memberstack application configuration

### How it works

1. Subscribe to this server
2. Enter your Memberstack Secret Key
3. Start managing your members from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_member_plans**: Get plans for a specific member
- **get_plan**: Get details for a specific plan
- **list_coupons**: List all discount coupons
- **list_custom_fields**: List member custom fields
- **list_members**: List all members
- **list_plans**: List all membership plans
- **list_promotions**: List active promotions
- **search_members**: Search members by email
- **get_application_info**: Get application details
- **get_member**: Get details for a specific member


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Memberstack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 members who joined."

**🤖 AI Agent:**
> Retrieving members... I found your most recent users, including 'john.doe@example.com' and 'jane.smith@domain.com'.

---

**👤 You:**
> "Show details for member ID 'mem_12345'."

**🤖 AI Agent:**
> Inspecting member... Member 'mem_12345' is currently on the 'Pro Plan' and has been active since last month.

---

**👤 You:**
> "What are my available membership plans?"

**🤖 AI Agent:**
> Querying plans... You have 3 plans configured: 'Free Tier', 'Monthly Pro', and 'Annual Enterprise'.


## Installation & Usage

To install and use the **Memberstack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/memberstack](https://vinkius.com/mcp/memberstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
