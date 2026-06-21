# The Cat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/the-cat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Access the world's largest collection of cat images, search by breed, and manage your favorites or votes directly from your AI agent.

## Description
Connect to **The Cat API** and bring feline intelligence to your AI workflows. Whether you need a specific breed image, want to upload your own cat, or manage a collection of favorites, this server provides full access to the most popular pet API.

### What you can do

- **Image Discovery** — Search for cat images with filters for size, type, and breed using `search_images`.
- **Breed Information** — List all known cat breeds or search for specific ones to get detailed characteristics via `list_breeds` and `search_breeds`.
- **Personal Collection** — Save images to your favorites with `create_favourite` and manage your voting history with `create_vote`.
- **Content Creation** — Upload your own cat images directly to the API via base64 using `upload_image`.

### How it works

1. Subscribe to this server
2. Enter your The Cat API Key
3. Start interacting with cat data from Claude, Cursor, or any MCP client.

### Who is this for?

- **Developers** — integrate cat content into applications or test image handling workflows.
- **Content Creators** — quickly find specific feline breeds for media projects.
- **Cat Enthusiasts** — manage a personal database of favorite cats through natural conversation.


## Available Tools
- **create_favourite**: Save an image to your favorites
- **create_vote**: Vote on an image (Up or Down)
- **get_favourites**: Retrieve your favorited images
- **get_image**: Get details for a specific image
- **get_votes**: Retrieve votes cast by your account
- **list_breeds**: Retrieve a list of all cat breeds
- **search_breeds**: Search for breeds by name
- **search_images**: Search for cat images
- **upload_image**: Upload your own cat image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **The Cat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 3 random cat images in GIF format."

**🤖 AI Agent:**
> I've found 3 cat GIFs for you! [Image 1: ID abc], [Image 2: ID def], [Image 3: ID ghi]. Would you like to see the details for any of these?

---

**👤 You:**
> "Find information about the 'Maine Coon' breed."

**🤖 AI Agent:**
> The Maine Coon is one of the largest domesticated breeds of cat. They are known for their intelligence and playful personalities. Their breed ID is 'mcoo'.

---

**👤 You:**
> "Show me my recently favorited cat images."

**🤖 AI Agent:**
> Retrieving your favorites... You have 5 favorited images. The most recent one is a beautiful Siamese cat (ID: xyz123).


## ❓ FAQ

**Q: How do I find high-quality cat images of a specific breed?**
You can use the `search_images` tool and specify the `size` as 'full' and `has_breeds` as true. To find a specific breed's ID first, use the `search_breeds` tool.

**Q: Can I see all the images I have previously favorited?**
Yes! Use the `get_favourites` tool. It will retrieve a list of all cat images you have saved to your account.

**Q: How do I cast a vote on a cat image?**
Use the `create_vote` tool. You'll need the `image_id` and a `value` (1 for an upvote, 0 for a downvote).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-cat](https://vinkius.com/mcp/the-cat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **The Cat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `the-cat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **The Cat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "the-cat": {
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
