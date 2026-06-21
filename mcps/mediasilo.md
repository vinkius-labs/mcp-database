# MediaSilo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mediasilo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Video collaboration and asset management via MediaSilo — manage projects, assets, and Quicklinks.

## Description
Connect your **MediaSilo** (Shift) account to any AI agent and take full control of your media asset management and collaboration through natural conversation.

### What you can do

- **Asset Management** — List all media assets, search by term, and fetch detailed metadata for videos and images
- **Project Organization** — Enumerate active projects, list folders, and inspect specific project configurations
- **Collaboration** — Manage Quicklinks for secure media sharing and review with your team and clients
- **User Inventory** — List authorized users and manage access within your MediaSilo workspace

### How it works

1. Subscribe to this server
2. Enter your MediaSilo API Key and API Secret
3. Start managing your media workflows from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_asset**: Get details for a specific asset
- **get_project**: Get details for a specific project
- **get_project_assets**: List all assets within a project
- **get_quicklink**: Get details for a specific Quicklink
- **list_assets**: ) from MediaSilo.

List all media assets
- **list_folders**: List folders within a project
- **list_projects**: List all projects
- **list_quicklinks**: List all Quicklinks
- **list_users**: List all users
- **search_assets**: Search for assets by term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MediaSilo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent assets in MediaSilo."

**🤖 AI Agent:**
> Retrieving assets... I found several recently added files, including 'Commercial_V3.mp4' and 'Product_Hero_Shot.jpg'.

---

**👤 You:**
> "Show folders for project 'Fall Campaign'."

**🤖 AI Agent:**
> Querying project folders... The 'Fall Campaign' project contains 3 folders: 'Raw Footage', 'Drafts', and 'Approved Masters'.

---

**👤 You:**
> "Search for assets matching 'logo'."

**🤖 AI Agent:**
> Searching... I found 5 assets matching 'logo', including high-res PNGs and vector files.


## ❓ FAQ

**Q: How do I find my MediaSilo API Key and Secret?**
Log in to MediaSilo, go to your Profile settings, and navigate to the API Keys section to generate a new key and secret.

**Q: What are Quicklinks?**
Quicklinks are a core MediaSilo feature used to securely share media for review without requiring the recipient to have a MediaSilo account.

**Q: Is my media data secure?**
Absolutely. Your credentials are encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mediasilo](https://vinkius.com/mcp/mediasilo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MediaSilo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mediasilo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MediaSilo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mediasilo": {
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
