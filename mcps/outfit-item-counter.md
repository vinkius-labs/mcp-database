# Outfit Item Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/outfit-item-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Quantify and analyze the composition of fashion outfits.

## Description
This MCP server provides tools to analyze the structure of fashion ensembles. You can use `count_total_items` to find the total number of pieces in an outfit, `count_items_by_category` to see the distribution of clothing types, and `verify_outfit_completeness` to ensure all necessary components like tops or bottoms are present. It also offers `get_outfit_summary` for a quick overview of an outfit's composition.


## Available Tools (4)
- **count_total_items**: Determines the total number of items present in a given outfit
- **get_outfit_summary**: Generates a high-level overview of an outfit's composition
- **verify_outfit_completeness**: Checks if an outfit meets specific composition requirements
- **count_items_by_category**: Provides a breakdown of how many items in an outfit belong to specific categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outfit Item Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many items are in outfit ID 'summer-001'?"

**🤖 AI Agent:**
> There are 3 items in outfit 'summer-001'.

---

**👤 You:**
> "Does outfit 'work-set-5' have both a top and a bottom?"

**🤖 AI Agent:**
> Yes, outfit 'work-set-5' is complete with both a top and a bottom.

---

**👤 You:**
> "Give me a summary of outfit 'evening-gala'."

**🤖 AI Agent:**
> Outfit 'evening-gala' contains 4 items: 1 Dress, 1 Pair of Shoes, 1 Clutch, and 1 Necklace.


## ❓ FAQ

**Q: How can I see how many items are in an outfit?**
You can use the `count_total_items` tool by providing the specific outfit ID.

**Q: Can I check if an outfit is missing any required pieces?**
Yes, the `verify_outfit_completeness` tool allows you to check if an outfit contains all required categories.

**Q: What kind of breakdown can I get for an outfit?**
The `count_items_by_category` tool provides a detailed mapping of how many items belong to each category like Tops, Bottoms, or Accessories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/outfit-item-counter](https://vinkius.com/en/ai-agent-connect/outfit-item-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outfit Item Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `outfit-item-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outfit Item Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outfit-item-counter": {
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
