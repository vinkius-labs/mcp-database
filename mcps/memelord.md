# MemeLord MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/memelord)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Generate viral memes and humorous visual content with AI that understands internet culture and creates shareable images instantly.

## Description
Connect your **MemeLord** account to any AI agent and generate memes programmatically through natural conversation.

### What you can do

- **Meme Generation** — Create memes by adding custom text to templates
- **Template Library** — Search and browse a massive library of viral meme templates
- **Image Manipulation** — Resize, crop, and add deep-fry effects to images
- **Text Overlay** — Add customizable top, bottom, and positioned text
- **Trending** — Access the latest trending meme formats

### How it works

1. Subscribe to this server
2. Enter your MemeLord API Key
3. Start generating memes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — generate viral content automatically
- **Community Managers** — create engaging memes for Discord/Slack
- **Developers** — build meme-generator bots and apps


## Available Tools (12)
- **check_api_health**: Verify Memelord API connectivity
- **generate_ai_meme**: Create a new meme using AI
- **generate_video_meme**: Usually delivered via webhook or async.

Generate a captioned video meme
- **edit_meme_with_ai**: Modify an existing meme using instructions
- **get_user_account_profile**: Get authenticated user profile
- **get_api_credit_usage**: Check remaining credits
- **get_api_version_info**: Retrieve API version and features
- **list_meme_categories**: g., Programming, Relationships, Sports).

Explore meme categories
- **list_my_collections**: List your saved meme collections
- **list_meme_templates**: List available classic meme templates
- **list_trending_memes**: See what is viral
- **list_configured_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MemeLord** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the 'Distracted Boyfriend' meme template."

**🤖 AI Agent:**
> Found templates matching 'Distracted Boyfriend': 1) Distracted Boyfriend (ID: 112126428, Text boxes: 3). 2) Distracted Girlfriend (ID: 142232). Template URL: https://img.memelord.com/112126428.jpg.

---

**👤 You:**
> "Generate a meme using the 'Drake' template."

**🤖 AI Agent:**
> Meme generated! ✅ Template: Drake Hotline Bling. Top text: 'Writing documentation'. Bottom text: 'Asking AI to write it'. URL: https://memelord.com/m/abc123xyz.jpg. Size: 800x800px.

---

**👤 You:**
> "Show the top 5 trending meme formats right now."

**🤖 AI Agent:**
> Trending Memes (24h): 1) 'Two Buttons' (Used 12K times today). 2) 'Change My Mind' (8K uses). 3) 'Expanding Brain' (6.5K uses). 4) 'Mocking Spongebob' (5K uses). 5) 'Disaster Girl' (4.2K uses).


## ❓ FAQ

**Q: Can I search for specific meme templates?**
Yes. Search the library by keywords (e.g., 'Drake Hotline Bling', 'Distracted Boyfriend') to find template IDs.

**Q: How does MemeLord authentication work?**
MemeLord uses Bearer authentication against `www.memelord.com/api/v1` using your API Key.

**Q: Can I add custom positioned text?**
Yes. You can add standard top/bottom text or specify exact X/Y coordinates for text boxes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/memelord](https://vinkius.com/mcp/memelord)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MemeLord** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `memelord` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MemeLord** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "memelord": {
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
