# Bannerbear (Image Gen) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bannerbear-image-gen)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate image and video generation via Bannerbear — create dynamic assets from templates and manage collections directly from your AI agent.

## Description
Connect your **Bannerbear** account to any AI agent and automate your design and marketing workflows through natural conversation.

### What you can do

- **Template Management** — List all available templates in your project and fetch detailed layer information using `list_templates` and `get_template`.
- **Dynamic Image Generation** — Create new images by applying text, color, or image modifications to templates with `create_image`.
- **Video Creation** — Generate videos based on video templates and input data frames using `create_video`.
- **Bulk Collections** — Process multiple images at once for high-volume workflows using the `create_collection` action.
- **Asset Retrieval** — Fetch the status and final URLs of your generated images using `get_image` to ensure they are ready for use.

### How it works

1. Subscribe to this server
2. Enter your Bannerbear API Key
3. Start generating visual content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — instantly generate social media banners, ad variations, and personalized content without opening a design tool.
- **Developers** — automate dynamic OG images or PDF generation directly from the code editor or terminal.
- **Content Creators** — quickly produce thumbnails and headers by simply describing the text and template you want to use.


## Available Tools (6)
- **get_template**: Retrieve the details of a specific template
- **list_templates**: Retrieve a list of templates in your project
- **create_collection**: Create multiple images at once as a collection
- **create_image**: Create an image based on a template
- **create_video**: Create a video based on a video template
- **get_image**: Retrieve the details of a previously created image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bannerbear (Image Gen)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Bannerbear templates."

**🤖 AI Agent:**
> I've retrieved your templates. You have 3 available: 'Promo Banner' (UID: abc-123), 'Twitter Post' (UID: def-456), and 'Product Card' (UID: ghi-789). Which one would you like to use?

---

**👤 You:**
> "Create an image using template abc-123 with the text 'Summer Sale' in the title layer."

**🤖 AI Agent:**
> I've initiated the image generation for template 'abc-123' with your modifications. The image UID is 'img-xyz-789'. You can check its status in a few moments.

---

**👤 You:**
> "Get the details and URL for image UID img-xyz-789."

**🤖 AI Agent:**
> The image is ready! You can view or download it here: https://bannerbear.com/outputs/img-xyz-789.png. The status is 'completed'.


## ❓ FAQ

**Q: How can I see which templates are available in my Bannerbear project?**
You can use the `list_templates` tool. It will return a list of all templates associated with your API key, including their names and unique UIDs.

**Q: Can I generate a video using this integration?**
Yes! Use the `create_video` tool by providing a video template UID and the necessary input data for the frames. The AI will handle the request and return the video details.

**Q: How do I check if my image has finished rendering?**
Use the `get_image` tool with the image UID. It will return the current status (e.g., 'completed') and the public URL of the image once it is ready.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bannerbear-image-gen](https://vinkius.com/mcp/bannerbear-image-gen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bannerbear (Image Gen)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bannerbear-image-gen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bannerbear (Image Gen)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bannerbear-image-gen": {
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
