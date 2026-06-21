# Pics.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/picsio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Organize and share creative assets with a digital asset management platform that tags, searches, and delivers files fast.

## Description
Connect your **Pics.io** account to any AI agent and take full control of your Digital Asset Management (DAM) orchestration through natural conversation. Pics.io provides a powerful platform for organizing large volumes of media, and this integration allows you to retrieve asset metadata, manage hierarchical collections, and track version histories directly from your chat interface.

### What you can do

- **Asset & Media Orchestration** — Search and list digital assets programmatically to ensure your media library is always accessible and synchronized.
- **Collection & Folder Intelligence** — Create and manage asset collections and retrieve detailed hierarchical metadata directly from the AI interface to maintain a high-fidelity DAM structure.
- **Metadata & Attribute Control** — Update asset titles, descriptions, and custom fields via natural language to drive better searchability and organizational efficiency.
- **Collaboration & Feedback Oversight** — Access and post comments on specific assets to maintain a clear audit trail of creative feedback using simple AI commands.
- **Operational Monitoring** — Track asset revisions and manage system-level metadata to ensure your creative workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Pics.io Personal Access Token from your integration settings
3. Start managing your media library from Claude, Cursor, or any MCP-compatible client

No more manual tagging or hunting for lost files in folders. Your AI acts as a dedicated asset curator or digital librarian.

### Who is this for?

- **Creative Directors & Designers** — quickly retrieve specific media assets and monitor design iterations without switching apps.
- **Marketing Teams** — automate the organization of campaign assets and track feedback loops via natural conversation.
- **Operations Managers** — streamline the retrieval of asset metadata and monitor organizational media health directly within the chat.


## Available Tools
- **add_comment**: Add a comment to an asset
- **create_collection**: Create a new collection
- **delete_collection**: Delete a collection
- **get_asset**: Get details for a specific asset
- **get_collection**: Get details for a specific collection
- **list_assets**: Optionally filter by collection ID.

List all digital assets
- **list_collections**: List all collections
- **list_comments**: List comments on an asset
- **list_revisions**: List asset revisions
- **search_assets**: Search for assets
- **update_asset**: Update asset metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pics.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all assets tagged with 'Summer 2024'."

**🤖 AI Agent:**
> I've retrieved your assets. You have 12 files matching 'Summer 2024', including 8 high-res photos and 4 videos. Would you like to see the details for any of them?

---

**👤 You:**
> "Search for all brand photography assets tagged with summer campaign 2025."

**🤖 AI Agent:**
> Found 34 assets matching "summer campaign 2025". 18 are high-resolution photos (4K+), 8 are social media graphics (1080x1080), 5 are banner images (1920x600), and 3 are video thumbnails. Top collection: "Beach Lifestyle" with 12 assets. All assets have approved brand guidelines tags. 6 were uploaded in the last 7 days by the creative team.

---

**👤 You:**
> "Create a new collection called Q3 Marketing Materials and move the approved assets into it."

**🤖 AI Agent:**
> Collection "Q3 Marketing Materials" created successfully (ID: col_8234). 27 approved assets have been organized into the collection: 14 product photos, 8 social templates, 3 presentation decks, and 2 brand guideline documents. The collection has been shared with the marketing team (view access) and the design team (edit access). A shareable link has been generated for external agency collaboration.


## ❓ FAQ

**Q: Can my AI automatically find the latest comments for a specific asset by its ID?**
Yes! Use the `list_comments` tool with the Asset ID. Your agent will respond with complete metadata for the conversation thread, including timestamps and author details in seconds.

**Q: How do I find my Pics.io Personal Access Token?**
Log in to Pics.io, navigate to **Account Settings** > **Integrations**, and look for the 'Personal Access Token' section to generate your unique secret key.

**Q: Can I search for assets across all collections?**
Absolutely. Use the `search_assets` tool with your query. The agent will return all matching files from your entire DAM, regardless of which collection they reside in.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/picsio](https://vinkius.com/mcp/picsio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pics.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `picsio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pics.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "picsio": {
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
