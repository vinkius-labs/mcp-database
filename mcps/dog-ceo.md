# Dog CEO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dog-ceo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Universal dog intelligence engine — get random dog images and breed data via AI.

## Description
Equip your AI agent with a source of canine joy via the **Dog CEO** MCP server. This integration provides access to the internet's biggest open-source collection of dog images. Your agent can retrieve random dog photos, list all available breeds and sub-breeds, and fetch breed-specific imagery. Whether you're building a pet-themed app, looking for visual assets, or just want to see a cute pup, your agent acts as a dedicated canine expert through natural conversation.

### What you can do

- **Random Dog Photos** — Get a random image of a dog from any breed.
- **Breed Exploration** — List all registered breeds and sub-breeds in the database.
- **Targeted Retrieval** — Fetch random images for specific breeds like 'retriever' or 'hound'.
- **Canine Intelligence** — Summarize breed data to identify origin and characteristics of different dogs.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start discovering dogs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Dog Lovers** — seeking a daily dose of cute canine content.
- **Developers** — wanting to add a fun and visual element to their AI interactions.
- **Content Creators** — looking for dog-related placeholders or assets.
- **Pet Stores & Vets** — access a reliable source of breed names and imagery for client materials.


## Available Tools (3)
- **get_dog_by_breed**: Get a dog image by breed
- **list_dog_breeds**: List all dog breeds
- **get_random_dog_image**: Get a random dog image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dog CEO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a random dog picture."

**🤖 AI Agent:**
> Coming right up! Here is a random dog for you. Isn't it adorable? I can also find images for specific breeds if you're interested.

---

**👤 You:**
> "Find 3 pictures of 'Golden Retrievers'."

**🤖 AI Agent:**
> Searching for Golden Retrievers... I've retrieved 3 high-quality images of this friendly and energetic breed. I can provide the direct image URLs for you.

---

**👤 You:**
> "List all sub-breeds for 'Hounds'."

**🤖 AI Agent:**
> Retrieving the list of sub-breeds for Hounds... I found several varieties including the Afghan, Basset, Blood, English, Ibizan, and Walker hounds. Would you like to see a picture of a specific one?


## ❓ FAQ

**Q: Can I get a photo of a specific breed like 'Husky'?**
Yes! Use the `get_dog_by_breed` tool and set the `breed` parameter to 'husky'. It will return a random image of that breed.

**Q: How do I list all available sub-breeds for a breed like 'Retriever'?**
Use the `list_sub_breeds` tool and provide 'retriever' as the breed. It will return a list of all sub-breeds like 'golden', 'flat-coated', etc.

**Q: Are there any copyrights on these dog images?**
The Dog CEO API sources images from various open repositories. While most are free to use, you should check the source links for specific licensing if using them for commercial purposes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dog-ceo](https://vinkius.com/mcp/dog-ceo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dog CEO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dog-ceo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dog CEO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dog-ceo": {
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
