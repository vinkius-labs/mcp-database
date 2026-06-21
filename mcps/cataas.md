# CatAAS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cataas)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Access the Cat as a Service (CATAAS) API to fetch random cat images, GIFs, and create custom cat memes with filters and text.

## Description
Bring the joy of cats to your AI interactions with the **CatAAS** MCP server. This integration allows any AI agent to fetch, filter, and customize cat images and GIFs directly from the CATAAS library.

### What you can do

- **Random Cats & GIFs** — Instantly fetch random cat images or animated GIFs to brighten your day or UI.
- **Tag Filtering** — Search for specific types of cats (e.g., 'orange', 'cute', 'sleeping') using the extensive tagging system.
- **Custom Text Overlays** — Create instant memes by overlaying custom text on cat images with adjustable fonts and colors.
- **Visual Filters** — Apply professional filters like blur, mono, or negate, and fine-tune brightness, saturation, and hue.
- **Metadata Exploration** — List all available tags and cat entries to discover the perfect visual for your needs.

### How it works

1. Subscribe to this server
2. Configure your access (no complex setup required)
3. Start requesting cats from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Add fun placeholders or dynamic cat content to applications during development.
- **Content Creators** — Quickly generate cat memes and visual assets using natural language.
- **Teams** — Lighten the mood in collaborative environments with random cat GIFs and images.


## Available Tools (7)
- **get_cat_by_tag**: Get a random cat filtered by tag
- **get_cat_with_tag_and_text**: Get a random cat with a specific tag and custom text
- **get_cat_with_text**: Get a random cat with custom text overlaid
- **get_random_cat**: Get a random cat image metadata
- **get_random_gif_cat**: Get a random animated cat GIF
- **list_cats**: List cats from the database
- **list_tags**: List all available tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CatAAS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a random cat image with a 'blur' filter."

**🤖 AI Agent:**
> I've fetched a blurred cat image for you. [Image ID: 596e421d844c04001011cc98]

---

**👤 You:**
> "Show me a cat with the tag 'orange' saying 'I am hungry'."

**🤖 AI Agent:**
> Here is an orange cat with your custom text overlay. [Image ID: 596e421f844c04001011cc9a]

---

**👤 You:**
> "List all available cat tags."

**🤖 AI Agent:**
> I've retrieved the tags. Popular ones include 'cute', 'orange', 'sleeping', 'black', and 'funny'. There are hundreds more available!


## ❓ FAQ

**Q: Can I add custom text to the cat images to create memes?**
Yes! Use the `get_cat_with_text` tool. You can specify the text, font size, and even font color to create the perfect cat meme in seconds.

**Q: How do I find out which tags are available for filtering?**
You can use the `list_tags` tool. It will return a comprehensive list of all categories and keywords used in the CatAAS database.

**Q: Is it possible to apply visual filters like 'blur' or 'grayscale'?**
Absolutely. Most tools like `get_random_cat` support a `filter` parameter where you can choose options like 'blur', 'mono', or 'negate'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cataas](https://vinkius.com/mcp/cataas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CatAAS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cataas` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CatAAS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cataas": {
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
