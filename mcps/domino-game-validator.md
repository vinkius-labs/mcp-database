# Domino Game Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/domino-game-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

A deterministic validator for standard double-six domino games.

## Description
This MCP server provides precise logic for validating moves in a standard double-six domino game. It handles complex rules including perpendicular doubles, spinner mechanics, and block game states. Use `validate_move` to check if a specific tile can be played at a given position, `get_legal_moves` to list all available options for a player, and `check_game_status` to determine if the game has ended via a win or a block.


## Available Tools (3)
- **check_game_status**: Evaluates whether the game has reached a conclusion (win, block, or ongoing)
- **get_legal_moves**: Identifies all possible legal moves a player can make from their current hand
- **validate_move**: Determines if a specific proposed move is legal given the current state of the game


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Domino Game Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it legal to play the 4-4 tile on the current board?"

**🤖 AI Agent:**
> Yes, the 4-4 tile can be played on the right end of the board.

---

**👤 You:**
> "What are my legal moves right now?"

**🤖 AI Agent:**
> You can play the 2-3 on the left end or the 5-6 on the right end.

---

**👤 You:**
> "Has the game ended yet?"

**🤖 AI Agent:**
> No, the game is still ongoing.


## ❓ FAQ

**Q: How do I check if a specific move is legal?**
You can use the `validate_move` tool by providing the current board state, the player's hand, and the proposed play details.

**Q: Can this tool identify all possible moves for a player?**
Yes, the `get_legal_moves` tool will return all valid tile IDs and their corresponding board positions, as well as whether a player must pass.

**Q: How does the tool handle the end of a game?**
The `check_game_status` tool evaluates the game state to identify if a player has won or if the game has reached a block state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/domino-game-validator](https://vinkius.com/ai-agent-connect/domino-game-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Domino Game Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `domino-game-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Domino Game Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "domino-game-validator": {
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
