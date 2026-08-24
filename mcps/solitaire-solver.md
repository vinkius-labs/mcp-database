# Solitaire Solver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/solitaire-solver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

A deterministic engine for validating Klondike solitaire moves and identifying legal plays.

## Description
This MCP server provides a precise decision engine for Klondike solitaire. It connects AI agents to the core logic required to play the game accurately. Use `validate_move` to check if a specific card movement follows color and rank rules, `get_legal_moves` to scan the entire tableau and waste for all available tactical opportunities, and `check_winnability` to determine if the current game state is solvable. It handles standard rules including 1-card or 3-card draw mechanics and empty column King requirements.


## Available Tools (3)
- **check_winnability**: Evaluates if the current state can lead to a win, assuming all cards are currently face-up
- **get_legal_moves**: Scans the entire current game state to list every possible valid move available to the player
- **validate_move**: Determines if a specific proposed card movement is legal under Klondike rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Solitaire Solver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it legal to move a Red 7 onto a Black 8 in the tableau?"

**🤖 AI Agent:**
> Yes, that is a legal move because the cards are of opposite colors and the ranks are sequential.

---

**👤 You:**
> "What are my legal moves right now?"

**🤖 AI Agent:**
> You can move the Ace of Spades to the foundation or the Red 5 to the Black 6 in column 2.

---

**👤 You:**
> "Can I win this game?"

**🤖 AI Agent:**
> Yes, there is a sequence of moves that allows all cards to be moved to the foundation.


## ❓ FAQ

**Q: How do I check if a move is legal?**
You can use the `validate_move` tool by providing the source and destination details to confirm if the move complies with Klondike rules.

**Q: Can this tool find all possible moves?**
Yes, the `get_legal_moves` tool scans the tableau, foundation, and waste to list every valid move available in the current state.

**Q: How does it determine if a game is winnable?**
The `check_winnability` tool simulates potential move paths to see if all cards can reach the foundation stacks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/solitaire-solver](https://vinkius.com/ai-agent-connect/solitaire-solver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Solitaire Solver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `solitaire-solver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Solitaire Solver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solitaire-solver": {
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
