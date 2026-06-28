# Lenormand Draw MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lenormand-draw)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [entertainment](../categories/entertainment.md)

Draw random Lenormand cards and discover traditional pair interpretations.

## Description
Connect your AI agent to the ancient wisdom of the Lenormand deck. This MCP server allows you to perform random single card draws using `draw_card`, generate multi-card spreads with `draw_spread`, and uncover deep insights through `interpret_pair` by analyzing how two cards interact. Perfect for automated readings, tarot-style analysis, and exploring the symbolic relationships within the 3-card Lenormand system.


## Available Tools (3)
- **draw_card**: Draw a single Lenormand card
- **draw_spread**: Draw a spread of cards
- **interpret_pair**: Interpret a pair of cards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lenormand Draw** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Draw a single Lenormand card for me."

**🤖 AI Agent:**
> The Rider has been drawn. This card represents news, speed, and arrivals.

---

**👤 You:**
> "Draw a 3-card spread for my day ahead."

**🤖 AI Agent:**
> Your spread consists of: 1. The Clover, 2. The Ship, and 3. The Anchor. This suggests a lucky journey or movement leading to stability.

---

**👤 You:**
> "What is the meaning of the Sun and the Moon together?"

**🤖 AI Agent:**
> The combination of The Sun and The Moon represents a period of great clarity, emotional fulfillment, and high visibility.


## ❓ FAQ

**Q: How do I draw a single card?**
Use the `draw_card` tool to receive a random card from the 36-card Lenormand deck, including its name and primary meaning.

**Q: Can I analyze multiple cards at once?**
Yes, you can use `draw_spread` to draw a sequence of cards and then use `interpret_pair` to find the combined meaning between adjacent cards.

**Q: What if a pair interpretation is not found?**
The `interpret_pair` tool uses a hardcoded database of traditional meanings. If the specific combination isn't in the catalog, it will return an error.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lenormand-draw](https://vinkius.com/mcp/lenormand-draw)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lenormand Draw** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lenormand-draw` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lenormand Draw** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lenormand-draw": {
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
