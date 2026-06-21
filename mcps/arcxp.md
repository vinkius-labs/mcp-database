# ArcXP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arcxp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate newsroom publishing via ArcXP — manage, search, and update articles, photos, and videos directly from any AI agent.

## Description
Connect your **ArcXP** environment to any AI agent and take full control of your newsroom CMS through natural conversation.

### What you can do

- **Content Management** — Create, fetch, update, and forcefully delete Arc Native Schema (ANS) stories directly without entering the Editor
- **Advanced Search** — Query your entire CMS library using powerful Elasticsearch-based syntax to find specific articles or historical reports
- **Media Library** — Search and retrieve high-resolution photo assets, thumbnails, and transcoding stream playlists for videos
- **Author Service** — List newsroom publishers, query specific reporter biographies, and manage author profiles

### How it works

1. Subscribe to this server
2. Enter your ArcXP Environment URL and Access Token
3. Start managing your digital publications from Claude, Cursor, or any MCP-compatible client

No more wrestling with complex ANS JSON schemas or slow CMS interfaces. Your AI acts as your ultimate publishing assistant.

### Who is this for?

- **Editors & Journalists** — quickly update breaking news, fetch related archive material, and orchestrate media without leaving your writing workflow
- **Media engineering teams** — automate bulk content updates and sanitize raw CMS payloads seamlessly
- **Digital publishers** — accelerate content velocity by letting AI structure, tag, and publish straight to your ArcXP tenant


## Available Tools
- **create_ans_content**: The payload_json MUST strictly comply with the requested Arc Native Schema (ANS) version.

Create new content in the Arc XP Content CMS
- **delete_ans_content**: Use with extreme caution as this destroys datacenter assets irreversibly.

Delete content from the Arc XP Content CMS
- **get_ans_content**: Returns the complete JSON payload matching the Arc Native Schema (ANS).

Fetch content from the Arc XP Content API
- **get_content_author**: Retrieve a publisher profile/author from Arc XP
- **get_photo_asset**: Retrieve a specific photo asset from Arc XP Media Library
- **get_video_asset**: Retrieve a specific video asset from Arc XP Video Center
- **list_content_authors**: List authors available in the Arc XP Author Service
- **search_ans_content**: Returns matching ANS JSON objects.

Search for content residing in the Arc XP Newsroom
- **search_photo_assets**: Search for photo assets in the Arc XP Media Library
- **update_ans_content**: Required to publish revisions to articles.

Update existing content in the Arc XP Content CMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ArcXP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the article JSON payload for ID MZG5X1..."

**🤖 AI Agent:**
> I've fetched the Arc Native Schema (ANS) payload for that article. It's a breaking news story titled 'Market Open Updates'. The author is Sarah Chen. Would you like me to update its tags or regenerate the core body paragraph?

---

**👤 You:**
> "Search our ArcXP newsroom for all stories containing 'Election 2024'..."

**🤖 AI Agent:**
> I ran the Elasticsearch query for 'Election 2024'. I found 32 published story nodes in the CMS. The most recent one is 'Debate Highlights' published 2 hours ago. I can summarize its ANS contents if needed.

---

**👤 You:**
> "List the first 20 registered editors in our CMS."

**🤖 AI Agent:**
> Here are the top active publisher profiles returned by the Author service. 1. Michael Doe (Global Editor), 2. Angela Ruiz (Sports Reporter)... Would you like to dig further into any of these contributor's published work?


## ❓ FAQ

**Q: Can my AI automatically rewrite an older story using Arc Native Schema and safely publish the update?**
Absolutely. Ask your agent to fetch a specific story by its ID. It understands the complex JSON structure of ANS, allows you to instruct it on what changes to make (e.g., 'Update the headline and add this new quote to paragraph 3'), and can dispatch an update command that preserves the content tree without breaking the CMS.

**Q: Is it possible to find specific high-res photos inside the ArcXP Media Library using natural language?**
Yes! Use the photo assets search action to query tags or captions using descriptive words. The AI fetches the asset ID, caption, credit strings, and directly accessible image URLs, letting you browse your editorial imagery seamlessly.

**Q: Can I query what articles a specific editor has authored?**
Yes! You can retrieve the Editor ID from the Author service and run an Elasticsearch query targeting their author object in the search tool. This quickly compiles all the CMS output for that specific reporter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcxp](https://vinkius.com/mcp/arcxp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ArcXP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `arcxp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ArcXP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arcxp": {
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
