# Cloudinary MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudinary)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Manage media assets via Cloudinary — track resources, monitor usage, and automate transformations directly from any AI agent.

## Description
Connect your **Cloudinary** account to any AI agent and take full control of your media library through natural conversation. Streamline how you manage, optimize, and distribute images and videos natively.

### What you can do

- **Resource Oversight** — List and retrieve details for all media resources including public IDs, formats, and secure URLs natively
- **Usage Intelligence** — Access core usage and quota reports for storage, bandwidth, and transformations flawlessly
- **Asset Logistics** — Monitor tags, folders, and transformations used across your media library securely
- **Search Management** — Perform advanced searches using complex expressions to find specific assets instantly flawlessly
- **Automation Logistics** — List configured upload presets to ensure consistent asset ingestion flawlessly
- **Content Control** — Permanently delete unwanted media resources directly from your chat interface flawlessly

### How it works

1. Subscribe to this server
2. Enter your Cloudinary API Key, API Secret, and Cloud Name
3. Start managing your media assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — monitor media libraries and organize assets using natural language
- **Developers** — audit asset transformations and verify delivery URLs without opening the dashboard
- **Marketing Teams** — quickly look up high-resolution assets and usage reports straight from their chat interface
- **Ops Teams** — verify storage utilization and monitor transformation quotas


## Available Tools (8)
- **delete_media_resource**: Permanently delete a media resource from the cloud
- **get_media_resource_details**: Get detailed information for a specific media resource
- **list_upload_presets**: List all configured upload presets
- **get_cloudinary_usage_report**: Retrieve core usage and quota information (Storage, Bandwidth, Transformations)
- **list_media_resources**: List all media resources (images, videos) in the cloud
- **list_media_tags**: List all tags used in the media library
- **list_media_transformations**: List all named and dynamic transformations
- **search_media_library**: Search for resources using a search expression


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloudinary** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all images in my Cloudinary library."

**🤖 AI Agent:**
> Retrieving your images... I found 5 items including 'product-hero-1', 'banner-winter-sale', and 'logo-white'. Would you like the secure URL for any of these?

---

**👤 You:**
> "What is my current Cloudinary storage usage?"

**🤖 AI Agent:**
> Checking your usage report... You are currently using 1.2GB of storage across 450 resources. This is approximately 12% of your plan's total capacity.

---

**👤 You:**
> "Search for all MP4 videos uploaded in the last 24 hours."

**🤖 AI Agent:**
> Searching media library... I found 2 MP4 videos uploaded since yesterday: 'demo-tutorial-v2' and 'customer-interview-final'. Would you like to see their metadata?


## ❓ FAQ

**Q: Can I see my bandwidth usage for this month?**
Yes! Use the `get_cloudinary_usage_report` tool. The agent will return core usage statistics, including current bandwidth and storage utilization compared to your plan limits.

**Q: How do I find all images tagged with 'summer'?**
Use the `search_media_library` tool with an expression like `tags:summer`. Your agent will fetch all matching resources directly from your library.

**Q: Where do I find my Cloudinary API Secret and Cloud Name?**
Log in to your Cloudinary Console. You can find your Cloud Name, API Key, and API Secret on the **Dashboard** main page under 'Account Details'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudinary](https://vinkius.com/mcp/cloudinary)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloudinary** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloudinary` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloudinary** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudinary": {
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
