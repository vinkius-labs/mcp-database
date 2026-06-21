# RandomDuck MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/randomduck)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Brighten your day with random duck images, GIFs, and HTTP status ducks for developers.

## Description
The **RandomDuck** MCP server connects your AI agent to the internet's favorite source of avian joy. Whether you need a random pick-me-up, a specific duck image, or a visual representation of an HTTP status code, this server has you covered.

### What you can do

- **Random Ducks** — Fetch random duck images or GIFs to brighten your day using `get_random_duck` or `get_quack`.
- **HTTP Status Ducks** — Visualize web development with ducks representing status codes like 404, 200, or 500 via `get_http_duck`.
- **Specific Retrieval** — Access a specific duck by its number and file type using `get_specific_duck`.
- **Duck Library** — Browse the entire collection of available filenames with `list_ducks`.
- **Contribute** — Upload your own duck images for review by Mod Mallard using `upload_duck`.

### How it works

1. Subscribe to this server
2. No API key is required for public access (enter 'public' as the token)
3. Start asking for ducks in Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Use HTTP ducks to make debugging more fun or to explain status codes to teammates.
- **Teams** — Share a random duck during standups or in chat to boost morale.
- **AI Enthusiasts** — Add a touch of personality and visual flair to your AI interactions.


## Available Tools
- **get_http_duck**: g., 404, 200, 500).

Get a duck representing an HTTP status code
- **list_ducks**: List all available duck filenames
- **get_quack**: Get a random duck (alias for random)
- **get_random_img_url**: Get a random duck image URL directly
- **get_random_duck**: Get a random duck image or GIF
- **get_specific_duck**: Get a specific duck image by number
- **upload_duck**: Upload a new duck image for review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RandomDuck** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a random duck image for me."

**🤖 AI Agent:**
> Quack! Here is a random duck for you: https://random-d.uk/api/32.jpg. Hope it makes your day better!

---

**👤 You:**
> "Show me the duck for HTTP 404 Not Found."

**🤖 AI Agent:**
> I've found the 404 duck! You can view it here: https://random-d.uk/api/http/404.jpg. It looks a bit lost, just like a 404 error.

---

**👤 You:**
> "List all available duck filenames."

**🤖 AI Agent:**
> I've retrieved the list. There are over 200 JPGs and 50 GIFs available, including special HTTP ducks for codes like 200, 403, and 500. Which one would you like to see?


## ❓ FAQ

**Q: Can I get a duck for a specific HTTP error code?**
Yes! Use the `get_http_duck` tool and provide the status code (e.g., 404 or 500). The agent will return the URL of a duck representing that specific HTTP state.

**Q: How do I see all the ducks available in the library?**
You can use the `list_ducks` tool. It will return lists of all available JPG and GIF filenames, as well as the supported HTTP status codes.

**Q: Can I upload my own duck images to the server?**
Absolutely. Use the `upload_duck` action with your base64 encoded image data. Your submission will be sent for review by the community moderators.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/randomduck](https://vinkius.com/mcp/randomduck)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RandomDuck** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `randomduck` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RandomDuck** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "randomduck": {
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
