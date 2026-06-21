# imgix (Real-time Image Processing) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/imgix-real-time-image-processing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Optimize and transform images via imgix — manage CDN sources, purge assets, and monitor origin connections.

## Description
Connect your **imgix** account to any AI agent and take full control of your real-time image processing and CDN infrastructure through natural conversation.

### What you can do

- **Source Orchestration** — List, create, and configure imgix sources to connect your origin storage (S3, GCS, Web Folder) to the CDN directly from your agent
- **Cache Management** — Purge specific assets from the imgix Edge network to force a re-fetch of original files and invalidate all processed derivatives instantly
- **Asset Monitoring** — Enumerate files in your origin sources and retrieve metadata including file paths, sizes, and content types
- **Operational Control** — Enable or disable specific sources to manage traffic flow and deployment windows for your visual media
- **Source Audit** — Retrieve detailed configuration for existing sources, including deployment types, custom domains, and origin status
- **Infrastructure Management** — Permanently remove unused sources or update caching attributes to optimize your image delivery pipeline

### How it works

1. Subscribe to this server
2. Enter your imgix API Key
3. Start managing your image CDN from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — verify origin connections and purge processed image derivatives after asset updates without leaving your IDE
- **SREs & DevOps** — monitor source availability and manage CDN deployment states through natural conversation
- **Digital Asset Managers** — audit asset libraries and organize origin storage connections across multiple imgix projects


## Available Tools
- **list_sources**: List all Imgix sources. Imgix is an image CDN that optimizes, resizes, and transforms images in real-time via URL parameters
- **get_source**: Get details of an Imgix source. Returns name, domain, deployment type, and status
- **create_source**: Create a new Imgix source. Connects your origin (S3, GCS, web folder) to Imgix CDN
- **update_source**: Update an Imgix source configuration. Modify name, caching, or deployment settings
- **enable_source**: Deploy/enable an Imgix source. Makes it live and serving images
- **disable_source**: Undeploy/disable an Imgix source. Stops serving images
- **purge**: Purge an asset from Imgix CDN cache. Removes original and all derivatives, forcing re-fetch
- **list_assets**: List assets in an Imgix source. Returns file paths, sizes, and content types
- **get_asset**: Get metadata of a specific asset in Imgix. Returns path, size, content type
- **delete_source**: Delete an Imgix source permanently


## 💬 Prompt Examples

Here are some examples of how you can interact with the **imgix (Real-time Image Processing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current imgix sources"

**🤖 AI Agent:**
> I've found 3 imgix sources: 'marketing-assets' (ID: src_123), 'e-commerce-products' (ID: src_456), and 'user-uploads' (ID: src_789). Which one would you like to inspect?

---

**👤 You:**
> "Purge this image from CDN: https://mycompany.imgix.net/logos/v2.png"

**🤖 AI Agent:**
> Purge request sent. I've invalidated 'logos/v2.png' across the global imgix Edge network. All processed versions of this file will now be re-fetched and transformed from your origin.

---

**👤 You:**
> "List the assets in the 'marketing-assets' source"

**🤖 AI Agent:**
> I've retrieved the assets for source 'src_123'. Recent files include '/banners/hero-winter.jpg', '/icons/social-bundle.svg', and '/product-shots/model-01.webp'. Total assets in this source: 1,245.


## ❓ FAQ

**Q: What happens when I purge an asset in imgix?**
Using the `purge` tool removes the cached version of the original image and ALL processed derivatives (resized, filtered, etc.) from imgix Edge nodes. This forces the system to re-fetch the file from your origin storage on the next request.

**Q: Can I connect my AWS S3 bucket to imgix using my agent?**
Absolutely. Use the `create_source` tool and provide your S3 origin base URL. Your agent will handle the backend orchestration to map your storage bucket to a new imgix CDN domain.

**Q: How do I check if a source is currently serving traffic?**
The `get_source` tool retrieves the real-time status of any imgix source. Your agent will return the deployment type and current state, so you'll know exactly if it's enabled and live.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/imgix-real-time-image-processing](https://vinkius.com/mcp/imgix-real-time-image-processing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **imgix (Real-time Image Processing)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `imgix-real-time-image-processing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **imgix (Real-time Image Processing)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "imgix-real-time-image-processing": {
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
