# DummyImage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dummyimage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate dynamic placeholder images for web development and design directly from your AI agent.

## Description
Connect to **DummyImage** to instantly generate placeholder images for your mockups, prototypes, and web layouts through natural conversation.

### What you can do

- **Custom Dimensions** — Generate images in any size (e.g., 300x250) or use standard keywords like `hd1080` or `medrect`.
- **Color Control** — Specify background and foreground hex colors to match your project's brand or UI theme.
- **Dynamic Text** — Add custom labels or descriptive text directly onto the generated image.
- **Format Selection** — Choose between common web formats including PNG, JPG, JPEG, and GIF.
- **Aspect Ratios** — Define specific ratios like 16:9 to test responsive containers.

### How it works

1. Subscribe to this server
2. Since this is a public service, enter 'PUBLIC' in the token field
3. Start generating image URLs directly in Claude, Cursor, or any MCP-compatible client

No more searching for placeholder services or manually creating empty boxes in design tools. Your AI acts as a rapid UI prototyper.

### Who is this for?

- **Web Developers** — quickly fill layout gaps with correctly sized images during frontend development.
- **UI/UX Designers** — generate specific placeholders for wireframes without leaving the workflow.
- **Product Managers** — visualize content blocks and banner placements during requirement gathering.


## Available Tools
- **generate_image**: Returns the generated image URL.

Generate a dummy image URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DummyImage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 300x250 placeholder image."

**🤖 AI Agent:**
> I've generated the placeholder for you. You can access it here: https://dummyimage.com/300x250/cccccc/000000.gif

---

**👤 You:**
> "Create a blue 16:9 image with white text saying 'Hero Banner'."

**🤖 AI Agent:**
> The 16:9 Hero Banner image has been created with a blue background and white text. URL: https://dummyimage.com/16:9/0000ff/ffffff.png?text=Hero+Banner

---

**👤 You:**
> "Generate a 100x100 PNG image for a profile placeholder."

**🤖 AI Agent:**
> I've generated a 100x100 PNG placeholder. Here is the link: https://dummyimage.com/100x100/cccccc/000000.png


## ❓ FAQ

**Q: Can I specify custom text to appear on the generated image?**
Yes! Use the `text` parameter in the `generate_image` tool to define any string you want to display in the center of the placeholder.

**Q: What image formats are supported by the generator?**
The `generate_image` tool supports `gif`, `jpg`, `jpeg`, and `png` formats. You can specify your preference using the `format` parameter.

**Q: Do I need to include the '#' symbol for hex colors?**
No. When using `background_color` or `foreground_color`, provide the hex code directly without the hash (e.g., '000000' for black or 'fff' for white).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dummyimage](https://vinkius.com/mcp/dummyimage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DummyImage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dummyimage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DummyImage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dummyimage": {
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
