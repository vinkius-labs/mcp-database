# Unsplash MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unsplash-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Manage your visual discovery — search photos, users, and collections via AI.

## Description
Empower your AI agent to orchestrate your entire visual ecosystem with **Unsplash**, the world's leading source of freely-usable images. By connecting Unsplash to your agent, you transform complex photo searches into a natural conversation. Your agent can instantly search for high-quality photos, audit user profiles, and retrieve curated collections without you ever touching a dashboard. Whether you are a content creator or a professional designer, your agent acts as a real-time visual curator, ensuring your projects are always powered by world-class imagery.

### What you can do

- **Photo Auditing** — Search for high-resolution images by keyword or orientation and retrieve detailed metadata, including descriptions and photographer info.
- **User Oversight** — Browse Unsplash user profiles and list all their uploaded photos to maintain a clear view of specific creators' portfolios.
- **Collection Management** — Search for and list curated collections to find themed imagery for any project instantly.
- **Visual Intelligence** — Retrieve random photos or specific photo statistics to understand image performance and reach.
- **Topic Discovery** — List curated topics on Unsplash to identify trending visual themes across the platform in real-time.

### How it works

1. Subscribe to this server
2. Enter your Unsplash Access Key (Client ID)
3. Start managing your visual assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Graphic Designers** — monitor image trends and retrieve specific photographer portfolios straight from your workflow.
- **Content Marketers** — verify if selected images align with brand aesthetic and retrieve high-quality alternatives.
- **Art Directors** — perform rapid audits of curated collections and identify new visual themes without manual logins.
- **Operations Leads** — automate visual data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools (10)
- **get_collection**: Get details for a specific collection
- **get_photo_stats**: Get statistics for a specific photo
- **get_photo**: Get details for a specific photo
- **get_random_photo**: Get a random high-quality photo
- **get_user_photos**: Get photos uploaded by a specific user
- **get_user**: Get details for a specific user
- **list_topics**: List curated topics on Unsplash
- **search_collections**: Search for curated collections on Unsplash
- **search_photos**: Search for high-quality photos on Unsplash
- **search_users**: Search for users on Unsplash


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unsplash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for landscape photos of 'Alpine mountains' on Unsplash."

**🤖 AI Agent:**
> I've retrieved high-quality landscape photos of Alpine mountains. Top matches include images by several professional photographers. Would you like the direct links to download them?

---

**👤 You:**
> "Get a random photo about 'Cyberpunk city'."

**🤖 AI Agent:**
> Random photo selected! I've found a stunning image of a neon-lit urban landscape. The photographer is 'John Doe' and you can access the full resolution via the provided URL.

---

**👤 You:**
> "List photos from user 'vinkius_creative'."

**🤖 AI Agent:**
> I've found 10 uploads from 'vinkius_creative'. The portfolio includes diverse themes like 'Nature' and 'Tech'. Would you like the metadata for the most recent upload?


## ❓ FAQ

**Q: How do I find my Unsplash Access Key?**
Log in to the [**Unsplash Developer portal**](https://unsplash.com/developers), create a new Application, and you will find your Access Key (Client ID) under the 'Keys' section. Copy and paste it below.

**Q: Can the agent filter photos by orientation?**
Yes. Use the `search_photos` tool providing the `orientation` parameter (landscape, portrait, or squarish). Your agent will return matching images instantly.

**Q: Is it possible to retrieve photo statistics via the agent?**
Yes. The `get_photo_stats` tool allows your agent to fetch real-time download and view counts for any specific photo by providing its Photo ID, helping you audit image reach.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unsplash-alternative](https://vinkius.com/mcp/unsplash-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unsplash** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `unsplash-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unsplash** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unsplash-alternative": {
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
