# Tarot Card Drawer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tarot-card-drawer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [entertainment](../categories/entertainment.md)

A cryptographically secure random generator for Tarot card draws, spreads, and deck analysis.

## Description
Connect your AI agent to the archetypal energies of the Tarot. This MCP server provides a cryptographically secure way to draw single cards, complex spreads, and inspect the composition of the 78-card deck. Use `draw_card` for immediate insights, `draw_spread` for structured readings like Past, Present, and Future, or `inspect_deck` to analyze the distribution of Major and Minor Arcana. Perfect for spiritual guidance, creative brainstorming, or archetypal analysis within Cursor, VS Code, Claude Desktop, and Windsurf.


## Available Tools (3)
- **draw_card**: Draw a single tarot card
- **draw_spread**: Draw a tarot spread
- **inspect_deck**: Inspect the tarot deck composition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tarot Card Drawer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Draw a single card for me to see what energy is surrounding me today."

**🤖 AI Agent:**
> The card drawn is The Magician. This represents manifestation, resourcefulness, and power. You have all the tools you need to succeed.

---

**👤 You:**
> "Perform a three-card spread for my past, present, and future."

**🤖 AI Agent:**
> Your Past: Three of Swords (heartbreak/sorrow). Your Present: The Star (hope/inspiration). Your Future: Ace of Pentacles (new opportunity/prosperity).

---

**👤 You:**
> "How many Major Arcana cards are in the deck?"

**🤖 AI Agent:**
> There are 22 Major Arcana cards in the deck.


## ❓ FAQ

**Q: How secure are the card draws?**
The server uses `crypto.getRandomValues()` to ensure that every draw is cryptographically secure and truly random.

**Q: Can I perform multi-card readings?**
Yes, you can use the `draw_spread` tool to generate a sequence of cards for structured readings like 'Past, Present, and Future'.

**Q: Does the tool support reversed cards?**
Yes, by setting the `includeReversed` parameter to true in `draw_card`, or `useReversals` in `draw_spread`, cards may appear in their inverted position.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tarot-card-drawer](https://vinkius.com/mcp/tarot-card-drawer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tarot Card Drawer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tarot-card-drawer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tarot Card Drawer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tarot-card-drawer": {
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
