# Openscreen MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openscreen)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openscreen-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openscreen-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-advertising](../categories/marketing-advertising.md)

Dynamic QR code management — generate and track smart QR codes for your assets via Openscreen.

## Description
Connect your **Openscreen** account to empower your AI agents with smart QR code capabilities. This server provides programmatic access to the Openscreen API for generating, managing, and tracking dynamic QR codes.

### What you can do

- **Dynamic QR Generation** — Create trackable QR codes for physical or digital assets
- **Project Organization** — Manage your QR codes across multiple projects and containers
- **Asset Management** — Link QR codes to specific assets like URLs, SKUs, or documents
- **Real-time Analytics** — Monitor scan data including location, device info, and scan times
- **Behavioral Control** — Update the intent of existing dynamic QR codes without changing the physical code

### How it works

1. Subscribe to this server
2. Enter your **Openscreen API Key** and **API Secret** from your dashboard
3. Start managing your smart interactions from Claude, Cursor, or any MCP client


## Available Tools
- **create_asset_with_qr**: Create an asset and its QR code
- **get_asset**: Get asset details
- **get_project**: Get project details
- **get_qr_code**: Get QR code details
- **list_assets**: List assets in a project
- **list_projects**: List all Openscreen projects
- **list_qr_codes**: List QR codes in a project
- **list_scans**: List scans for a QR code
- **update_qr_code_intent**: Update QR code intent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Openscreen** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my Openscreen projects."

**🤖 AI Agent:**
> Fetching projects... I've found 3 projects: 'Marketing Q1', 'Product Launch', and 'Inventory Tracking'.


## Installation & Usage

To install and use the **Openscreen** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openscreen](https://vinkius.com/mcp/openscreen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
