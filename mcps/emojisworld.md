# EmojisWorld MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emojisworld)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Universal emoji intelligence — search emojis, list categories, and get random icons via AI.

## Description
Equip your AI agent with a comprehensive source of visual expression through the **EmojisWorld** MCP server. This integration provides instant access to thousands of emojis organized by category. Your agent can search for emojis by keyword, retrieve random icons for creative inspiration, and explore the complete index of emoji categories. Whether you are enhancing user interfaces, automating social media content, or just finding the perfect reaction, your agent acts as a dedicated emoji curator through natural conversation.

### What you can do

- **Emoji Search** — Find specific emojis by name or related keywords across a massive database.
- **Random Inspiration** — Retrieve a random emoji to spark creativity in messages or designs.
- **Category Indexing** — List all available emoji categories like 'Smileys', 'Animals', and 'Food'.
- **Direct Character Access** — Get the actual emoji character along with its name and category metadata.
- **Visual Auditing** — Summarize and group emojis to identify themes for branding or content strategies.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start discovering emojis from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **UX/UI Designers** — quickly find emojis for mockups and interface designs.
- **Social Media Managers** — enhance posts and engagement with relevant visual icons.
- **Developers** — integrate dynamic emoji features into their AI applications.
- **Creative Writers** — add visual flair and personality to their digital content.


## Available Tools (3)
- **list_emoji_categories**: g., Smileys, Animals).

List all emoji categories
- **get_random_emoji**: Get a random emoji
- **search_emojis**: g., heart, smile).

Search for emojis by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EmojisWorld** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a random emoji."

**🤖 AI Agent:**
> Sure! Here is a random one for you: 🍕 (Pizza). Would you like another one or are you looking for something specific?

---

**👤 You:**
> "Search for emojis related to 'space'."

**🤖 AI Agent:**
> Searching for space-themed emojis... I found 🚀 (Rocket), 🪐 (Ringed Planet), 🌌 (Milky Way), and 👩‍🚀 (Astronaut). Would you like to see the full list of metadata?

---

**👤 You:**
> "List all emoji categories."

**🤖 AI Agent:**
> Retrieving the categories... I've found 9 main groups including Smileys & People, Animals & Nature, Food & Drink, Activities, and Travel & Places. Which category would you like to explore?


## ❓ FAQ

**Q: Can I search for a 'rocket' emoji?**
Yes! Use the `search_emojis` tool with the query 'rocket'. It will return the 🚀 emoji along with its details.

**Q: How can I see all emojis in the 'Food' category?**
Use the `list_emojis_by_category` tool and provide the category number or name. For 'Food', use category ID 4.

**Q: Is it possible to get a random emoji for inspiration?**
Yes. The `get_random_emoji` tool retrieves a single random emoji character and its metadata from the entire database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emojisworld](https://vinkius.com/mcp/emojisworld)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EmojisWorld** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emojisworld` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EmojisWorld** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emojisworld": {
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
