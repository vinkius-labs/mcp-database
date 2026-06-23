# Pixabay API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pixabay-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Search stock media — audit images and videos via AI.

## Description
Empower your AI agent to orchestrate your entire visual content and media auditing workflow with the **Pixabay API**, the authoritative source for high-quality, royalty-free stock media. By connecting Pixabay to your agent, you transform complex media searches into a natural conversation. Your agent can instantly search for thousands of images and videos, audit tag distributions, and retrieve direct download links without you ever touching a stock photo portal. Whether you are building marketing collateral or conducting visual research, your agent acts as a real-time creative consultant, ensuring your media is always stunning and properly licensed.

### What you can do

- **Image Auditing** — Search for thousands of high-resolution images by keyword and retrieve detailed metadata, including tags and user info.
- **Video Oversight** — Audit free video clips to understand the temporal distribution of visual content for your projects instantly.
- **Media Discovery** — Filter results by image type (e.g., photo, illustration, vector) or orientation to identify relevant assets for your layout.
- **Visual Intelligence** — Retrieve high-quality web previews and direct links to assist in deep-dive media classification.
- **Operational Monitoring** — Check API status to ensure your media research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your Pixabay API Key
3. Start managing your media intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Designers** — monitor media trends and retrieve high-quality visual metadata straight from your workflow.
- **Marketing Managers** — verify asset availability and audit creative patterns without manual searching.
- **Web Developers** — perform rapid audits of placeholder images and identify relevant media markers through natural language.
- **Operations Leads** — automate media data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools (3)
- **check_api_status**: Check if the Pixabay service is operational
- **search_pixabay_images**: Search for free high-quality images on Pixabay
- **search_pixabay_videos**: Search for free high-quality videos on Pixabay


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pixabay API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for high-quality images of 'sunset over mountains' using Pixabay."

**🤖 AI Agent:**
> I've retrieved several stunning images of sunsets! Notable previews include mountain landscapes with vibrant colors. I can provide the direct links to the high-resolution files if you'd like.

---

**👤 You:**
> "Find illustrations of 'robot working' in 'horizontal' orientation."

**🤖 AI Agent:**
> I've identified several horizontal illustrations of robots! They are categorized as 'illustration' type and match your search criteria. I can assist you with the user metadata and tags for each image.

---

**👤 You:**
> "Search for free videos about 'nature' on Pixabay."

**🤖 AI Agent:**
> I've retrieved several nature videos from the Pixabay catalog! They feature landscapes and wildlife with various durations. I can provide the unique video IDs and direct links to assist in your project.


## ❓ FAQ

**Q: How do I find my Pixabay API Key?**
Log in to your [**Pixabay account**](https://pixabay.com/api/docs/), and you will find your API Key in the 'Parameters' section of the API documentation page. Copy and paste it below.

**Q: Can I search for videos specifically?**
Yes. Use the `search_pixabay_videos` tool to retrieve free video clips and their associated metadata from the Pixabay catalog.

**Q: Are illustrations and vectors included?**
Yes. When using the `search_pixabay_images` tool, you can specify the `image_type` parameter as 'illustration' or 'vector' to filter your results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pixabay-api](https://vinkius.com/mcp/pixabay-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pixabay API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pixabay-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pixabay API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pixabay-api": {
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
