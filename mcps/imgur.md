# Imgur MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/imgur)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Manage Imgur content — upload images, organize albums, and browse the gallery directly from your AI agent.

## Description
Connect your **Imgur** account to any AI agent to automate image hosting, album organization, and gallery interactions through natural language.

### What you can do

- **Image Management** — Upload images via binary data, base64, or URLs, and update titles or descriptions instantly
- **Album Orchestration** — Create, delete, and manage albums, including adding multiple images to specific collections
- **Gallery Exploration** — Search the global Imgur gallery, fetch viral content, and manage your account favorites
- **Account Insights** — Retrieve public profile data, submissions, and private account settings
- **Engagement** — Create, delete, and vote on comments within the Imgur community

### How it works

1. Subscribe to this server
2. Enter your Imgur Client ID (and optional Access Token for private actions)
3. Start managing your media assets from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Creators** — quickly upload and organize assets for social media or blogs
- **Developers** — manage application screenshots and assets directly from the terminal or IDE
- **Social Media Managers** — monitor gallery trends and manage community engagement efficiently


## Available Tools
- **add_images_to_album**: Add images to an existing album
- **create_album**: Create a new album
- **create_comment**: Create a new comment on an item
- **delete_album**: Delete an album with a given ID
- **delete_comment**: Delete a comment
- **delete_image**: Delete an image
- **get_account_gallery_favorites**: Get the user's gallery favorites
- **get_account_settings**: Get the current user's account settings (requires access token)
- **get_account_submissions**: Get images and albums submitted to the gallery by the user
- **get_account**: Get standard user information for an Imgur account
- **get_album**: Get information about a specific album
- **get_comment**: Get information about a specific comment
- **get_gallery**: Get the Imgur gallery
- **get_image**: Get information about a specific image
- **search_gallery**: Search the gallery for images and albums
- **submit_to_gallery**: Submit an image or album to the gallery
- **update_image**: Update the title or description of an image
- **upload_image**: Upload a new image
- **vote_comment**: Vote on a comment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Imgur** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Imgur gallery for 'vintage photography' and show me the results."

**🤖 AI Agent:**
> I've searched the gallery for 'vintage photography'. I found several high-quality matches, including a collection of 1950s street scenes (ID: abc123) and a set of film portraits (ID: def456).

---

**👤 You:**
> "Upload this image URL to Imgur: https://example.com/photo.jpg"

**🤖 AI Agent:**
> The image has been successfully uploaded! You can view it at https://imgur.com/xyz789. The image hash is xyz789.

---

**👤 You:**
> "Get the details and description for image hash xyz789."

**🤖 AI Agent:**
> Fetching details for xyz789... The image is titled 'Sunset over Mountains', has 1,200 views, and is currently set to public visibility.


## ❓ FAQ

**Q: Can I upload an image just by providing a web URL?**
Yes! Use the `upload_image` tool and set the `type` parameter to 'url'. The agent will fetch the image and host it on Imgur for you.

**Q: How do I create a private album for my project assets?**
Use the `create_album` tool and set the `privacy` parameter to 'hidden' or 'secret'. You can also provide an initial list of image IDs.

**Q: Can I see my private account settings through the AI?**
Yes, provided you have supplied an Access Token. Use the `get_account_settings` tool to retrieve your current account configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/imgur](https://vinkius.com/mcp/imgur)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Imgur** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `imgur` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Imgur** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "imgur": {
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
