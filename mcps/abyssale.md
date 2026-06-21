# Abyssale MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abyssale)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automated creative production — generate dynamic images, banners, and personalized visuals via AI.

## Description
Connect your **Abyssale** account to your AI agent to automate your creative workflow. From generating personalized banners for email marketing to creating dynamic social media visuals on-the-fly, your agent manages creative production through natural conversation.

### What you can do

- **Automated Image Generation** — Create high-quality images from your Abyssale designs by overriding text and image layers via API
- **Design Exploration** — List and retrieve details of your design templates, including available elements and formats
- **Dynamic Image URLs** — Generate permanent URLs that create personalized visuals in real-time based on query parameters
- **Batch Production** — Handle high-volume creative requests for marketing campaigns without manual design work
- **Visual Personalization** — Scale your visual content by personalizing every element for your target audience instantly

### How it works

1. Subscribe to this server
2. Enter your Abyssale API Key
3. Start generating and managing your creative assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — automate personalized visual content for emails, ads, and social media
- **E-commerce Managers** — generate dynamic product banners and promotional visuals at scale
- **Developers** — integrate automated image generation into custom applications and workflows
- **Content Creators** — scale visual production without spending hours in design tools


## Available Tools (4)
- **list_designs**: List all Abyssale designs
- **get_design**: Get design template details
- **generate_image**: Generate an image from a design
- **create_dynamic_image_url**: Create a dynamic image URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Abyssale** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Abyssale design templates."

**🤖 AI Agent:**
> I've retrieved your design templates. You have 12 designs available, including 'Welcome Banner', 'Product Promo', and 'Event Invite'. Which one would you like to explore?


## ❓ FAQ

**Q: How do I personalize a design template via the agent?**
Use the `generate_image` tool and provide the `designId` along with an `elements` object containing the layer names and the new values (text or image URLs) you want to apply.

**Q: What is a Dynamic Image URL?**
It's a permanent URL that generates an image in real-time when accessed. You can pass personalization parameters directly in the query string, making it perfect for dynamic content in emails.

**Q: Does the API support high-volume batch processing?**
Yes, it supports asynchronous processing for batch generation. It integrates via webhooks to notify external systems when your generated images or HTML5 banners are ready.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abyssale](https://vinkius.com/mcp/abyssale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Abyssale** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `abyssale` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Abyssale** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "abyssale": {
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
