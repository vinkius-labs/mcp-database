# Microsoft App Store MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/microsoft-app-store)
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


## ❓ FAQ

**Q: How do I create the Azure AD application?**
Go to Partner Center > Account settings > User management > Azure AD applications to associate an application and generate a secret.

**Q: Which permissions are required?**
The application must be associated with your Partner Center account and granted the 'Manager' or 'Developer' role.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/microsoft-app-store](https://vinkius.com/mcp/microsoft-app-store)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Microsoft App Store** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `microsoft-app-store` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Microsoft App Store** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "microsoft-app-store": {
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
