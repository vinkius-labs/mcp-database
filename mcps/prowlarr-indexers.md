# Prowlarr (Indexers) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prowlarr-indexers)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/prowlarr-indexers-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/prowlarr-indexers-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Prowlarr indexers—list, add, test, and monitor health status of your Usenet and Torrent indexers directly from your AI agent.

## Description
Connect your **Prowlarr** instance to any AI agent and take full control of your indexer management through natural conversation. This server allows you to orchestrate your Usenet and Torrent indexers without leaving your workspace.

### What you can do

- **Indexer Overview** — List all configured indexers and retrieve detailed configurations for specific ones using their IDs.
- **Health Monitoring** — Instantly check the health status of all indexers to identify connection issues or failures.
- **Configuration Management** — Add new indexers, update existing settings, or remove indexers that are no longer needed.
- **Schema Discovery** — Fetch templates and required fields for various indexer types (Newznab, Torznab, etc.) to ensure correct setup.
- **Pre-save Testing** — Test indexer configurations before saving them to ensure credentials and URLs are valid.

### How it works

1. Subscribe to this server
2. Enter your Prowlarr URL and API Key
3. Start managing your indexers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Home Lab Enthusiasts** — Monitor and maintain your media automation stack without opening multiple web interfaces.
- **Media Server Admins** — Quickly troubleshoot indexer failures and update API keys or URLs on the fly.
- **DevOps Engineers** — Automate the provisioning and testing of indexer configurations via AI-driven workflows.


## Available Tools
- **add_indexer**: Use get_indexer_schema to find the correct fields.

Add a new indexer
- **delete_indexer**: Delete an indexer
- **get_indexer**: Get details of a specific indexer
- **list_indexers**: List all configured indexers
- **get_indexer_schema**: Get templates for all supported indexers
- **get_indexer_status**: Get indexer health status
- **test_indexer**: Test an indexer configuration
- **update_indexer**: Update an existing indexer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prowlarr (Indexers)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my configured indexers in Prowlarr."

**🤖 AI Agent:**
> I've retrieved your indexers. You have 4 configured: 'RARBG' (ID: 1), '1337x' (ID: 2), 'DrunkenSlug' (ID: 5), and 'NinjaCentral' (ID: 8). Would you like to check the status of any of these?

---

**👤 You:**
> "Check the health status of all my indexers."

**🤖 AI Agent:**
> I've checked the health status. Most indexers are healthy, but 'RARBG' is reporting a connection timeout. Would you like me to test its configuration?

---

**👤 You:**
> "Get the schema for adding a new Newznab indexer."

**🤖 AI Agent:**
> I've fetched the schema for Newznab indexers. The required fields include 'baseUrl', 'apiKey', and 'categories'. I can help you format the JSON to add it once you have those details.


## Installation & Usage

To install and use the **Prowlarr (Indexers)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prowlarr-indexers](https://vinkius.com/mcp/prowlarr-indexers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
