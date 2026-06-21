# Storylane MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/storylane)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/storylane-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/storylane-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Interactive, personalized product demos.

## Description
The Storylane MCP server connects your AI agent directly to your demo infrastructure. Query demo completion rates, create personalized demo links for prospects, and sync engagement data natively.


## Available Tools
- **create_demo_link**: Generate a new trackable demo link
- **get_demo_analytics**: Get engagement metrics for a specific demo
- **get_demo**: Get metadata and status for a specific demo
- **get_me**: Get information about the current authenticated user
- **get_session_details**: Get detailed information for a specific viewer session
- **get_workspace_info**: Retrieve metadata about the current Storylane workspace
- **list_demo_links**: Retrieve all active links associated with a specific demo
- **list_demos**: List all published demos in the workspace
- **list_sessions**: List granular session analytics for demo viewers
- **list_teams**: List teams within the workspace
- **list_users**: List all users and their roles in the workspace
- **update_demo_link**: Update settings for an existing demo link


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Storylane** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our active product demos."

**🤖 AI Agent:**
> You have 3 active demos: 'Platform Overview', 'Analytics Deep Dive', and 'Admin Panel'.

---

**👤 You:**
> "Create a personalized link for 'Analytics Deep Dive' for Acme Corp."

**🤖 AI Agent:**
> Personalized link generated: storylane.io/demo/acme-analytics-123

---

**👤 You:**
> "Show the completion rate for the 'Platform Overview' demo."

**🤖 AI Agent:**
> The 'Platform Overview' demo currently has a 68% completion rate with an average view time of 4m 12s.


## Installation & Usage

To install and use the **Storylane** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/storylane](https://vinkius.com/mcp/storylane)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
