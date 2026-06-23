# Fluxiom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fluxiom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage digital assets, organize with tags, and oversee collections via AI agents with Fluxiom DAM.

## Description
Connect your **Fluxiom** account to any AI agent to automate your Digital Asset Management (DAM) and sharing workflows. Fluxiom provides a streamlined platform for storing, organizing, and distributing your brand's files. This MCP server enables you to manage your asset library, apply organizational tags, and oversee your sharing portals (Stages) directly through natural conversation.

### What you can do

- **Asset Management** — List all digital assets, fetch detailed metadata, and update or delete files instantly.
- **Dynamic Tagging** — Create and apply organizational tags to categorize your library programmatically.
- **Branded Portals** — Access and list your sharing portals or 'Stages' to monitor how your files are being distributed.
- **Version Control** — Retrieve the complete version history for any asset to track updates and changes.
- **Search & Filter** — Efficiently locate specific files using full-text search and tag-based filtering.
- **Account Oversight** — Fetch detailed account attributes and metadata to maintain full context of your DAM environment.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fluxiom Subdomain and API Key
3. Start managing your digital assets directly from your AI agent


## Available Tools (9)
- **create_tag**: Create a new tag
- **delete_asset**: Remove an asset
- **get_account_details**: Get account attributes
- **get_asset**: Get asset details
- **get_asset_versions**: Get asset version history
- **list_assets**: List digital assets
- **list_stages**: List branded portals (Stages)
- **list_tags**: List organizational tags
- **update_asset**: Update asset metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fluxiom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all digital assets tagged with 'Marketing'."

**🤖 AI Agent:**
> Searching assets... I found 5 files tagged with 'Marketing', including your Q4 brand assets.

---

**👤 You:**
> "Show me the version history for asset ID '12345'."

**🤖 AI Agent:**
> Retrieving versions... Asset '12345' has 3 versions. The latest update was on March 15th.

---

**👤 You:**
> "Add the tag 'Archive' to the asset 'Logo_Final.png'."

**🤖 AI Agent:**
> Updating asset... The 'Archive' tag has been successfully applied to 'Logo_Final.png'.


## ❓ FAQ

**Q: How do I get an API Key for Fluxiom?**
You can find your API token in your Fluxiom user account settings under the Integrations or API section.

**Q: What is a 'Stage' in Fluxiom?**
A 'Stage' is a branded portal or collection used to share curated sets of files with external partners or clients.

**Q: Can I manage file versions using the agent?**
Yes, the 'get_asset_versions' tool allows you to retrieve the complete history of updates for any specific digital asset.

**Q: Does Fluxiom support high-res previews?**
Yes, Fluxiom generates previews for common image, video, and document formats automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fluxiom](https://vinkius.com/mcp/fluxiom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fluxiom** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fluxiom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fluxiom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fluxiom": {
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
