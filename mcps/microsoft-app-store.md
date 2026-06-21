# Microsoft App Store MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/microsoft-app-store)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/microsoft-app-store-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/microsoft-app-store-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Microsoft Store apps — track submissions, add-ons, and package flights via the Submission API.

## Description
Connect your **Microsoft Store** developer account to automate app management tasks. This server interfaces with the **Microsoft Store Submission API** for real-time visibility and control.

### What you can do

- **App Inventory** — List and inspect all applications registered in your account
- **Submission Tracking** — Monitor the status of pending or completed app submissions
- **Add-on Management** — List in-app products and their metadata
- **Flight Coordination** — View package flights for beta testing or staged rollouts

### How it works

1. Subscribe to this server
2. Enter your **Azure Tenant ID**, **Client ID**, and **Client Secret**
3. Start managing your store presence from Claude, Cursor, or any MCP client


## Available Tools
- **get_addon**: Get details for a specific add-on
- **get_application**: Get details for a specific application
- **get_flight**: Get details for a specific package flight
- **get_submission**: Get details for a specific submission
- **list_addons**: List add-ons for an application
- **list_applications**: List all applications in your Microsoft Store account
- **list_flights**: List package flights for an application
- **list_submissions**: List submissions for an application


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microsoft App Store** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Microsoft Store apps."

**🤖 AI Agent:**
> Fetching applications... I've found 3 apps registered: 'Photo Editor Pro', 'TaskMaster', and 'Game Hub'.

---

**👤 You:**
> "What is the status of the latest submission for 'TaskMaster'?"

**🤖 AI Agent:**
> Checking submissions... The latest submission for 'TaskMaster' (ID #115292) is currently 'PendingPublication'.


## Installation & Usage

To install and use the **Microsoft App Store** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/microsoft-app-store](https://vinkius.com/mcp/microsoft-app-store)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
