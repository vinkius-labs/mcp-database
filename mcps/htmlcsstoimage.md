# HTMLCSSToImage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/htmlcsstoimage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate high-quality images and PDFs from HTML/CSS or URLs directly from your AI agent.

## Description
Connect **HTMLCSSToImage** to your AI agent to automate visual content creation. Convert code snippets or live websites into PNG, JPG, WebP, or PDF files using a simple and powerful API.

### What you can do

- **HTML to Image** — Render custom HTML and CSS snippets into pixel-perfect images instantly.
- **URL Screenshots** — Capture full-page or element-specific screenshots from any public URL with browser-grade precision.
- **Template Management** — Create, edit, and use reusable templates to generate dynamic images with variable data.
- **Batch Processing** — Generate or delete up to 25 images in a single request for high-volume automated workflows.
- **Advanced Customization** — Control viewports, device scaling, Google Fonts, dark mode, and specific CSS selectors for cropping.

### How it works

1. Subscribe to this server
2. Enter your HCTI User ID and API Key
3. Start generating visuals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Automate the creation of social sharing images (Open Graph), dynamic reports, or UI mockups.
- **Marketers** — Generate personalized banners, email visuals, and promotional content at scale.
- **Content Creators** — Turn code snippets or web data into shareable visual assets without leaving your chat interface.


## Available Tools (10)
- **batch_create_images**: Create up to 25 images in one request
- **batch_delete_images**: Delete multiple images at once
- **create_image_from_template**: Create an image from a template
- **create_image**: Either html or url is required.

Create an image from HTML/CSS or a URL
- **create_template**: Create a reusable image template
- **delete_image**: Permanently remove an image
- **edit_template**: Edit an existing image template
- **get_image**: Can apply cropping and resizing via query parameters.

Retrieve a generated image file or its metadata
- **get_usage**: Check account usage
- **list_images**: List generated images


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HTMLCSSToImage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a PNG image from this HTML: <h1 style='color: blue;'>Hello MCP</h1>"

**🤖 AI Agent:**
> I've generated your image. You can view it here: https://hcti.io/v1/image/example_id.png

---

**👤 You:**
> "Take a full-page screenshot of https://github.com/trending"

**🤖 AI Agent:**
> Capturing the full page... Done! Here is the link to your screenshot of GitHub Trending.

---

**👤 You:**
> "Show me my current API usage for HTMLCSSToImage."

**🤖 AI Agent:**
> You have used 150 out of 1000 images this month. Your account is in good standing.


## ❓ FAQ

**Q: Can I capture just a specific element of a webpage instead of the whole page?**
Yes! Use the `create_image` tool and provide a CSS `selector`. The API will find that specific element and crop the resulting image to its dimensions.

**Q: How do I generate multiple images at once for a bulk project?**
You can use the `batch_create_images` tool. It allows you to send an array of variations and optional default settings to generate up to 25 images in a single API call.

**Q: How can I check my remaining API credits and usage?**
Simply run the `get_usage` tool. It will return your current account statistics, including total images generated and your remaining balance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/htmlcsstoimage](https://vinkius.com/mcp/htmlcsstoimage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HTMLCSSToImage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `htmlcsstoimage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HTMLCSSToImage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "htmlcsstoimage": {
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
