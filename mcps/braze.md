# Braze MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/braze)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/braze-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/braze-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage customer engagement via Braze — track users, list campaigns, and trigger canvases directly from any AI agent.

## Description
Connect your **Braze** customer engagement platform to any AI agent and orchestrate your marketing automation and user tracking workflows through natural conversation.

### What you can do

- **User Orchestration** — Track new user attributes and events, identify anonymous users, or permanently delete user profiles for compliance.
- **Campaign Management** — List all your marketing campaigns, retrieve detailed metadata, and instantly trigger API-based campaign sends to specific users.
- **Canvas (Journey) Control** — List and inspect multi-step Canvases, and trigger users to enter specific Canvas workflows.
- **Data Export** — Programmatically export user profile data by their external IDs.

### How it works

1. Subscribe to this server
2. Enter your Braze REST API Key and Base URL (e.g., https://rest.iad-01.braze.com)
3. Start managing your customer journeys from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_canvas_details**: Get details of a specific Canvas
- **track_user**: Track user attributes or events
- **trigger_campaign**: Trigger an API-triggered campaign
- **trigger_canvas**: Trigger a Canvas journey
- **delete_user**: Delete a user by external ID
- **export_user_ids**: Export profile data for specific users
- **get_campaign_details**: Get details of a specific campaign
- **identify_user**: Identify a user (merge alias to external ID)
- **list_campaigns**: List all campaigns
- **list_canvases**: List all Canvases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Braze** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns in Braze."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active campaigns: 'Welcome Series' (ID: camp_1), 'Abandoned Cart' (ID: camp_2), and 'Holiday Promo' (ID: camp_3).

---

**👤 You:**
> "Track user 'usr_992' with attribute {'loyalty_tier':'Gold'}."

**🤖 AI Agent:**
> The user attribute 'loyalty_tier: Gold' has been successfully tracked for user 'usr_992'.

---

**👤 You:**
> "List all Canvases configured in the workspace."

**🤖 AI Agent:**
> Retrieving Canvases... You have 2 active Canvases: 'Onboarding Journey' (ID: can_1) and 'Win-back Flow' (ID: can_2).


## Installation & Usage

To install and use the **Braze** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/braze](https://vinkius.com/mcp/braze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
