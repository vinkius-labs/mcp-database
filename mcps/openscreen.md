# Openscreen MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openscreen)
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


## ❓ FAQ

**Q: What is the difference between static and dynamic QR codes?**
Static codes are fixed. Dynamic codes allow you to change the destination (Intent) without reprinting the physical code, and they provide scan tracking.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openscreen](https://vinkius.com/mcp/openscreen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Openscreen** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `openscreen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Openscreen** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openscreen": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
