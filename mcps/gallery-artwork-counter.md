# Gallery Artwork Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gallery-artwork-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Track and analyze artwork inventory and display metrics across multiple art galleries.

## Description
This MCP server provides tools to manage and query art gallery inventories. It allows AI agents to retrieve total inventory counts, monitor pieces currently on display, generate reports on large collections, and analyze the distribution of art between display and storage. Use `get_all_galleries_report` to identify major collections or `get_gallery_inventory_summary` to get a complete breakdown of a specific gallery's holdings.


## Available Tools (4)
- **get_all_galleries_report**: Answers which galleries have the largest collections
- **get_artwork_status_distribution**: Answers the breakdown of art statuses (Display vs Storage) within a specific gallery
- **get_gallery_display_metrics**: Answers how many pieces of art are currently visible to the public in this gallery
- **get_gallery_inventory_summary**: Answers how many artworks are currently in the inventory for a specific gallery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gallery Artwork Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many artworks are currently in the inventory for gallery 'G-123'?"

**🤖 AI Agent:**
> Gallery G-123 has a total inventory of 150 artworks, with 45 on display and 105 in storage.

---

**👤 You:**
> "Which galleries have at least 50 artworks in their collection?"

**🤖 AI Agent:**
> The galleries with at least 50 artworks are: Modern Art Hub (85), Heritage Gallery (62), and Urban Canvas (55).

---

**👤 You:**
> "What is the status distribution for gallery 'G-456'?"

**🤖 AI Agent:**
> In gallery G-456, there are 30 artworks on display and 20 artworks in storage.


## ❓ FAQ

**Q: How does the inventory count work?**
The inventory count includes all artworks currently owned by the gallery, which consists of pieces on display and those in storage. Sold artworks are excluded from these counts.

**Q: Can I see which galleries have the most art?**
Yes, you can use the `get_all_galleries_report` tool to list galleries and their inventory sizes, optionally filtering by a minimum size.

**Q: What is the difference between display count and inventory count?**
The display count only includes artworks currently visible to the public, while the inventory count includes both displayed art and art held in storage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gallery-artwork-counter](https://vinkius.com/en/ai-agent-connect/gallery-artwork-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gallery Artwork Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gallery-artwork-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gallery Artwork Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gallery-artwork-counter": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
