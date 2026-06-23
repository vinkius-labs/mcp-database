# Cincopa MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cincopa)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Manage video and media galleries via Cincopa — track assets, trigger uploads, and monitor engagement directly from any AI agent.

## Description
Connect your **Cincopa** account to any AI agent and take full control of your video and media management through natural conversation. Streamline how you host and distribute content.

### What you can do

- **Gallery Oversight** — List and retrieve details for all media galleries and folders natively
- **Asset Intelligence** — Access detailed metadata for videos, images, and audio files flawlessly
- **Upload Automation** — Retrieve temporary upload URLs to push new content to your platform securely
- **Template Management** — List available gallery templates to ensure consistent branding flawlessly
- **Content Control** — Create new galleries and delete unwanted assets directly from your chat interface flawlessly
- **Engagement Monitoring** — Monitor media performance and usage metadata directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Cincopa API Token (obtained from API & Developers settings)
3. Start managing your media assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — monitor video libraries and manage gallery structures using natural language
- **Marketing Teams** — audit media performance and metadata without opening the dashboard
- **E-learning Specialists** — quickly look up asset IDs and organize course content straight from their chat interface
- **Developers** — verify media uploads and metadata integration during technical setup


## Available Tools (8)
- **create_new_gallery**: Create a new media gallery using a template
- **delete_media_asset**: Permanently delete a media asset from the account
- **get_asset_metadata**: Get detailed metadata for a specific media asset
- **get_gallery_details**: Get detailed information for a specific gallery
- **get_media_upload_url**: Retrieve a temporary URL for uploading new media files
- **list_cincopa_assets**: List all media assets (videos, images, audio)
- **list_cincopa_galleries**: List all media galleries in the account
- **list_cincopa_templates**: List available gallery templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cincopa** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my video galleries in Cincopa."

**🤖 AI Agent:**
> Retrieving your galleries... I found 5 items: 'Product Demos', 'Marketing Assets', 'Internal Training', and 2 others. Which one would you like to see the contents of?

---

**👤 You:**
> "Show me the metadata for asset RID 'AAAAtAURG'."

**🤖 AI Agent:**
> Checking asset AAAAtAURG... This is a MP4 video titled 'Feature Update'. It is 45MB, has a 1080p resolution, and was last modified yesterday.

---

**👤 You:**
> "Create a new gallery called 'Customer Interviews' using the 'Video Portal' template."

**🤖 AI Agent:**
> Creating gallery 'Customer Interviews'... The gallery has been successfully created. You can now use its FID (A4KANh__rQ_m) to add media assets to it.


## ❓ FAQ

**Q: Can I get a direct link to upload a video through the agent?**
Yes! Use the `get_media_upload_url` tool. The agent will return a temporary URL that you can use to POST your video file directly to Cincopa's servers.

**Q: How do I see the metadata for a specific image or video?**
Use the `get_asset_metadata` tool with the unique Resource ID (rid). Your agent will fetch detailed info like resolution, format, and size.

**Q: Where do I find my Cincopa API Token?**
Log in to your Cincopa account and navigate to **Settings > API & Developers**. You can generate and copy your personal API token from there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cincopa](https://vinkius.com/mcp/cincopa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cincopa** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cincopa` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cincopa** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cincopa": {
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
