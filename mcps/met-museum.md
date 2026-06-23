# Met Museum MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/met-museum)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Explore the Metropolitan Museum of Art's collection—search for artworks, list departments, and retrieve detailed object metadata and images.

## Description
Connect to **The Metropolitan Museum of Art's Open Access API** and bring over 5,000 years of art history to your AI agent. Access data on more than 470,000 artworks from the Met collection for use in research, creative projects, or education.

### What you can do

- **Advanced Search** — Find objects using keywords, filtering by artist, culture, medium, or geographic location.
- **Object Metadata** — Retrieve comprehensive details for specific artworks, including titles, dates, materials, and dimensions.
- **Department Browsing** — List all 19 museum departments (e.g., Egyptian Art, The American Wing) to narrow your exploration.
- **Image Access** — Identify objects with public domain images and retrieve high-resolution URLs for visual reference.
- **Collection Auditing** — List valid object IDs and filter by recent updates to stay synchronized with the museum's digital archives.

### How it works

1. Subscribe to this server
2. Enter your API identifier (use 'PUBLIC' if no specific key is required by your proxy)
3. Start exploring art history from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Educators & Students** — Quickly find primary source materials and metadata for art history research.
- **Designers & Creatives** — Search for public domain inspiration and high-quality imagery based on specific historical periods or mediums.
- **Data Scientists** — Analyze collection trends and metadata across different cultures and eras.


## Available Tools (4)
- **list_departments**: List all valid departments
- **get_object**: Get detailed record for a specific object
- **list_objects**: List all valid Object IDs available
- **search_objects**: Search for objects matching a query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Met Museum** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Van Gogh' paintings that are currently on view in the museum."

**🤖 AI Agent:**
> I found several works by Vincent van Gogh currently on view. Notable Object IDs include 436535 (Wheat Field with Cypresses) and 436533 (Self-Portrait with a Straw Hat). Would you like the full details for any of these?

---

**👤 You:**
> "List all museum departments and their IDs."

**🤖 AI Agent:**
> The Met has 19 departments. Some examples include: 'American Decorative Arts' (ID: 1), 'Egyptian Art' (ID: 10), and 'Modern Art' (ID: 21). I can use these IDs to filter your future searches.

---

**👤 You:**
> "Get the detailed record for object ID 436535."

**🤖 AI Agent:**
> Object 436535 is 'Wheat Field with Cypresses' by Vincent van Gogh (1889). It is an oil on canvas from the European Paintings department. I have also retrieved the primary image URL for you.


## ❓ FAQ

**Q: How can I search for artworks by a specific artist that have images available?**
You can use the `search_objects` tool. Set the `q` parameter to the artist's name and set `hasImages` to `true`. This will return a list of Object IDs matching those criteria.

**Q: Can I get the full historical record and image URL for a specific piece of art?**
Yes! Use the `get_object` tool with the specific `objectID`. It returns detailed metadata including the artist, medium, dimensions, and `primaryImage` or `additionalImages` URLs.

**Q: How do I find out which departments exist in the Met Museum?**
Use the `list_departments` tool. It will provide a complete list of all valid departments along with their unique `departmentId`, which you can then use to filter your searches.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/met-museum](https://vinkius.com/mcp/met-museum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Met Museum** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `met-museum` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Met Museum** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "met-museum": {
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
