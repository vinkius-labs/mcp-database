# Unkey API Management MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unkey-api-management)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/unkey-api-management-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/unkey-api-management-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage and verify your user API keys via Unkey — create, revoke, and track usage directly from any AI agent.

## Description
Connect your AI agent to **Unkey**, the robust platform for issuing and managing API keys at scale. This integration allows you to oversee your API infrastructure, manage developer keys, and audit verification analytics through natural conversation.

### What you can do

- **Key Issuance** — Create new API keys for your users with custom prefixes, metadata, and ownership
- **Verification** — Instantly verify if a key is valid and check its remaining credits or usage limits
- **Lifecycle Management** — List all keys for an API, update their status, or permanently revoke them
- **Infrastructure Oversight** — List and inspect your defined APIs and their configurations
- **Usage Analytics** — Retrieve detailed verification stats to monitor how your developers are using your services

### How it works

1. Subscribe to this server
2. Enter your **Unkey Root Key** (found in your Unkey dashboard settings)
3. Start managing your API key infrastructure via chat

### Who is this for?

- **DevOps Engineers** — quickly audit and manage API keys during system maintenance
- **Product Managers** — track API adoption and usage trends through verification analytics
- **Customer Support** — verify developer keys and reset or update them based on support tickets


## Available Tools
- **create_api_key**: Create a new API key for your users
- **revoke_api_key**: Permanently delete (revoke) an API key
- **get_api_details**: Get detailed information for a specific API
- **get_verification_analytics**: Retrieve usage analytics for your API keys
- **list_apis**: Retrieve a list of all APIs in your Unkey project
- **list_api_keys**: List all API keys associated with a specific API ID
- **update_api_key**: Update an existing API key
- **verify_api_key**: Verify if an API key is valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unkey API Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all APIs in my Unkey project."

**🤖 AI Agent:**
> Fetching APIs... I found 2 APIs: 'Public Storefront' (ID: api_123) and 'Admin Dashboard' (ID: api_456). Which one would you like to manage?

---

**👤 You:**
> "Verify the API key 'user_sk_abcdef123'."

**🤖 AI Agent:**
> Verification result: Key is VALID. Owner: 'user_789'. Remaining credits: 4,500. This key is associated with the 'Premium Plan'.


## Installation & Usage

To install and use the **Unkey API Management** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unkey-api-management](https://vinkius.com/mcp/unkey-api-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
