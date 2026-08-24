# Bingo Card Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bingo-card-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Generate reproducible 5x5 Bingo cards and validate game states.

## Description
This MCP server provides a deterministic toolkit for 75-ball Bingo. Use `generate_card` to create a reproducible 5x5 grid using a unique ID (1-10000). You can use `validate_card` to ensure a grid follows standard rules, or `check_game_state` to evaluate if a player has achieved patterns like a line, four corners, or a blackout based on called numbers.


## Available Tools (3)
- **check_game_state**: Evaluates a card against a list of drawn numbers to determine progress and wins
- **generate_card**: Generates a reproducible 5x5 Bingo card based on a specific ID
- **validate_card**: Checks if a provided grid configuration is a legally formed Bingo card


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bingo Card Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a bingo card with ID 500."

**🤖 AI Agent:**
> Here is your generated Bingo card for ID 500: [B: 2, 7, 12, 1, 15 | I: 18, 22, 29, 16, 30 | N: 31, 40, FREE, 35, 44 | G: 46, 55, 50, 59, 48 | O: 61, 70, 65, 75, 68]

---

**👤 You:**
> "Check if card 500 wins with numbers 2, 7, 12, 1, 15, 18, 22, 29, 16, 30, 31, 40, 35, 44, 46, 55, 50, 59, 48, 61, 70, 65, 75, 68 and the center free space."

**🤖 AI Agent:**
> The card is a winner! The pattern 'blackout' has been completed.

---

**👤 You:**
> "Is this grid a valid bingo card: [[1, 16, 31, 46, 61], [2, 17, 32, 47, 62], [3, 18, 33, 48, 63], [4, 19, 34, 49, 64], [5, 20, 35, 50, 65]]?"

**🤖 AI Agent:**
> No, the grid is invalid because the center cell is not a 'FREE' space.


## ❓ FAQ

**Q: How do I get the same card every time?**
Use the `generate_card` tool with the same `cardId` between 1 and 10000 to reproduce the exact same 5x5 grid.

**Q: What winning patterns are supported?**
The `check_game_state` tool supports checking for a 'line', 'four_corners', and 'blackout'.

**Q: Can I verify if a custom grid is valid?**
Yes, use the `validate_card` tool to check if a 5x5 grid adheres to the standard 75-ball Bingo constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bingo-card-generator](https://vinkius.com/ai-agent-connect/bingo-card-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bingo Card Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bingo-card-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bingo Card Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bingo-card-generator": {
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
