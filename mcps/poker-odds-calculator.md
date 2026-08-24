# Poker Odds Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/poker-odds-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Deterministic Texas Hold'em odds calculator for hand strength, outs, and win probabilities.

## Description
This MCP server provides precise mathematical analysis for Texas Hold'em players. Use `calculate_hand_strength` to identify your current hand rank, `analyze_outs` to find cards that improve your position, `calculate_win_probability` to estimate your chances against multiple opponents, and `calculate_pot_odds` to determine if a call is mathematically profitable based on the pot size.


## Available Tools (4)
- **analyze_outs**: Identifies how many cards in the deck will improve the player's hand
- **calculate_hand_strength**: Determines the current best poker hand ranking based on available cards
- **calculate_pot_odds**: Determines the mathematical necessity of calling a bet
- **calculate_win_probability**: Predicts the percentage chance of winning against a specific number of opponents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Poker Odds Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my hand strength with hole cards [As, Ks] and community cards [Ad, Kc, 7d]?"

**🤖 AI Agent:**
> You have Two Pair, Aces and Kings.

---

**👤 You:**
> "How many outs do I have with [8s, 9s] and community cards [Ts, Js, 2d]?"

**🤖 AI Agent:**
> You have 8 outs to a straight.

---

**👤 You:**
> "What is my win probability with [Ah, Ad] against 3 opponents with community cards [2s, 7c, Jd, 4h, 9s]?"

**🤖 AI Agent:**
> Your win probability is 72.4%.


## ❓ FAQ

**Q: How does the win probability calculation work?**
The `calculate_win_probability` tool uses combinatorial analysis to compare your hand against the possible ranges of your opponents.

**Q: Can I calculate pot odds for any bet size?**
Yes, by using `calculate_pot_odds`, you can input any current pot size and call amount to see if the move is profitable.

**Q: What cards can I input?**
You can input standard Texas Hold'em cards using rank and suit notation, such as 'As' for Ace of Spades or '7d' for 7 of Diamonds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/poker-odds-calculator](https://vinkius.com/ai-agent-connect/poker-odds-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Poker Odds Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `poker-odds-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Poker Odds Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "poker-odds-calculator": {
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
