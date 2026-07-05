# Poker Odds Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/poker-odds-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Calculate exact probabilities, equities, and outs for Texas Hold'em and Omaha.

## Description
A high-precision combinatorial engine for poker players. This MCP server provides tools to calculate exact hand probabilities, win/loss equity against multiple opponents, identify specific outs to improve your hand, and evaluate pot odds for mathematically sound decision-making. Use `calculate_hand_probabilities` to see the distribution of possible final ranks, `calculate_win_loss_equity` to estimate your share of the pot, `identify_outs` to find cards that complete your draws, and `evaluate_pot_matches` to determine if a call is profitable.


## Available Tools (4)
- **evaluate_pot_odds**: Provides a recommendation on whether to call a bet
- **calculate_hand_probabilities**: Determines the probability distribution of all possible final hand ranks
- **identify_outs**: Identifies cards that improve the player's hand to a target strength
- **calculate_win_loss_equity**: Estimates the likelihood of winning, losing, or splitting the pot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Poker Odds Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have Ace of Spades and King of Diamonds. The board is 2s, 7h, 10c. What are my probabilities for different hand ranks in Texas Hold'em?"

**🤖 AI Agent:**
> Based on your cards [As, Kd] and the board [2s, 7h, 10c], your probabilities are: High Card: 85.4%, One Pair: 13.2%, Two Pair: 1.4%.

---

**👤 You:**
> "I'm playing Omaha with [As, Ks, Qs, Js]. The board is [2s, 7h, 10c]. How many outs do I have to make a flush?"

**🤖 AI Agent:**
> You have 9 outs remaining in the deck to complete your flush.

---

**👤 You:**
> "The pot is $100 and I need to call a $20 bet. My win probability is 15%. Should I call?"

**🤖 AI Agent:**
> No, you should not call. The pot odds are 6:1, but your required equity is 16.67%.


## ❓ FAQ

**Q: Does this tool use Monte Carlo simulations?**
No. This engine uses exact combinatorial mathematics to evaluate all possible remaining card combinations, ensuring 100% accuracy for both Texas Hold'em and Omaha.

**Q: How can I find which cards will complete my flush draw?**
You can use the `identify_outs` tool. By providing your hole cards, the current board, and setting the target rank to 'Flush', it will return a list of all specific cards in the deck that complete your draw.

**Q: Can I calculate my equity against multiple opponents?**
Yes. The `calculate_win_loss_equity` tool allows you to specify the number of opponents to estimate your probability of winning, losing, or splitting the pot.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/poker-odds-calculator](https://vinkius.com/mcp/poker-odds-calculator)
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
