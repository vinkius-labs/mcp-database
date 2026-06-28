# Tarot Spread Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tarot-spread-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured tarot readings using predefined spreads like Celtic Cross and Horseshoe.

## Description
The Tarot Spread Generator connects AI agents to the mystical art of tarot. By using tools like `list_spread_templates`, `get_position_definitions`, and `generate_new_reading`, users can instantly create structured readings. Whether you are looking for a quick 3-card 'Past-Present-Future' insight or a deep dive with the 10-card 'Celtic Cross', this MCP server automates the randomized drawing process, ensuring each card is unique within the spread and providing clear thematic meanings for every position.


## Available Tools (3)
- **list_spread_templates**: Provides an overview of all available tarot spread configurations
- **generate_new_reading**: Executes a randomized drawing of cards for a specific spread template
- **get_position_definitions**: Explains the meaning of each slot within a specific tarot spread


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tarot Spread Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the available tarot spreads."

**🤖 AI Agent:**
> The following spreads are available: Celtic Cross (10 cards), Horseshoe (7 cards), Past-Present-Future (3 cards), and Astrological Year (12 cards).

---

**👤 You:**
> "What does the 'Past' position mean in a 3-card spread?"

**🤖 AI Agent:**
> In the Past-Present-Future spread, the first position represents the energies and events that have shaped your current situation.

---

**👤 You:**
> "Generate a new reading using the Horseshoe spread."

**🤖 AI Agent:**
> Your Horseshoe reading has been generated (ID: 7a2b-9c3d). The cards drawn are: The Magician (Position 1), The High Priestess (Position 2), and The Empress (Position 3)...


## ❓ FAQ

**Q: What spreads are available?**
You can use `list_spread_templates` to see all available configurations, including the Celtic Cross, Horseshoe, and Past-Present-Future spreads.

**Q: How do I know what each card position means?**
Use the `get_position_definitions` tool by providing the name of the spread to see the thematic meaning of every slot in that layout.

**Q: Can I generate a new reading immediately?**
Yes, simply call `generate_new_reading` with your chosen spread name to get a unique randomized draw.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tarot-spread-generator](https://vinkius.com/mcp/tarot-spread-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tarot Spread Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tarot-spread-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tarot Spread Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tarot-spread-generator": {
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
