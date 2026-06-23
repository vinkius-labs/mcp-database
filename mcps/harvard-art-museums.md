# Harvard Art Museums MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harvard-art-museums)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search museum collections — audit art objects, artists, and exhibitions via AI.

## Description
Empower your AI agent to orchestrate your entire art history research and collection auditing workflow with **Harvard Art Museums**, the authoritative source for global art metadata. By connecting the Harvard Art Museums API to your agent, you transform complex object searches into a natural conversation. Your agent can instantly search for art objects across various periods, audit artist portfolios, and retrieve detailed exhibition metadata without you ever touching a museum portal. Whether you are conducting academic research or scouting visual inspiration, your agent acts as a real-time art curator, ensuring your data is always grounded in official, museum-verified records.

### What you can do

- **Object Auditing** — Search for thousands of art objects by title or artist and retrieve detailed metadata, including periods and medium info.
- **Artist Oversight** — Browse artist profiles and identify their contributions to the museum collection to maintain a clear view of their work.
- **Exhibition Discovery** — Query upcoming and historical exhibitions to understand the thematic distribution of art displays instantly.
- **Visual Intelligence** — Retrieve direct links to high-quality primary images for any museum object to maintain visual context.
- **Gallery Monitoring** — List all galleries within the Harvard Art Museums to understand the organizational layout of the collections.

### How it works

1. Subscribe to this server
2. Enter your Harvard Art Museums API Key
3. Start managing your art intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Art Historians & Scholars** — monitor collection data and retrieve official metadata straight from your workflow.
- **Curators & Researchers** — verify object details and audit artist distributions without manual searches.
- **Designers & Creatives** — perform rapid audits of visual assets and discover historical inspiration through natural language.
- **Operations Leads** — automate art data querying to orchestrate cross-functional educational teams smoothly.


## Available Tools (6)
- **check_api_status**: Check if the Harvard Art Museums API is operational
- **get_object_details**: Get full details for a specific art object by ID
- **list_museum_galleries**: List all galleries within the Harvard Art Museums
- **search_exhibitions**: Search for exhibitions hosted by the Harvard Art Museums
- **search_museum_objects**: Search for art objects in the Harvard Art Museums collection
- **search_museum_people**: Search for artists and people related to the museum collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harvard Art Museums** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for art objects by 'Vincent van Gogh' in Harvard Art Museums."

**🤖 AI Agent:**
> I've retrieved 10 works by Vincent van Gogh in the collection. Notable objects include 'Self-Portrait' and 'The Three Sunflowers'. Would you like the image links or full metadata for any of these?

---

**👤 You:**
> "Show details for exhibition with name 'Modernism'."

**🤖 AI Agent:**
> I've identified several exhibitions related to Modernism. Notable matches include 'French Modernism' and 'American Modernist Prints'. I can provide the dates and gallery locations if you'd like.

---

**👤 You:**
> "List all galleries in the museum."

**🤖 AI Agent:**
> I've scanned the gallery catalog. There are over 50 galleries listed, categorized by floor and theme (e.g., 'Ancient Art', 'Contemporary Art'). I can provide the specific gallery IDs for further object searches.


## ❓ FAQ

**Q: How do I find my Harvard Art Museums API Key?**
Request a free API Key by filling out the form on the [**Harvard Art Museums API portal**](https://harvardartmuseums.org/collections/api). Your key will be sent to you via email.

**Q: Can the agent show images of the art?**
Yes. The `search_museum_objects` and `get_object_details` tools retrieve primary image URLs for objects where available in the digital collection.

**Q: Is it possible to search for specific artists?**
Yes. Use the `search_museum_people` tool providing the artist's name. Your agent will return their profile ID and identifying metadata instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harvard-art-museums](https://vinkius.com/mcp/harvard-art-museums)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Harvard Art Museums** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `harvard-art-museums` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Harvard Art Museums** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "harvard-art-museums": {
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
