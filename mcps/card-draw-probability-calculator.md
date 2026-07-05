# Card Draw Probability Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/card-draw-probability-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Calculate the mathematical likelihood of drawing specific cards in TCGs like Magic: The Gathering or Yu-Gi-Oh.

## Description
This MCP server provides specialized tools for TCG and CCG players to calculate precise probabilities using hypergeometric distribution. Use `calculate_draw_probability` to find the chance of hitting target cards in your next draws, or `get_distribution_table` for a full breakdown of all possible outcomes. The `evaluate_mulligan_decision` tool helps you decide whether to keep your current hand or take a mulligan based on expected quality, while `track_deck_progression` allows you to update your deck state after scrying or thinning effects.


## Available Tools (4)
- **track_deck_progression**: Track changes to the deck after thinning or scrying
- **get_distribution_table**: Generate a full probability distribution table
- **calculate_draw_probability**: Calculate the probability of drawing target cards
- **evaluate_mulligan_decision**: Evaluate whether to keep a hand or take a mulligan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Card Draw Probability Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my chances of drawing at least 2 lands in my next 7 cards if I have 24 lands in a 60-card deck?"

**🤖 AI Agent:**
> The probability of drawing at least 2 lands is approximately 85.3%.

---

**👤 You:**
> "Should I mulligan my current hand? My hand quality score is 0.5, the penalty is 1, initial size was 7, deck is 60 with 10 targets, and success threshold is 0.6."

**🤖 AI Agent:**
> MULLIGAN. The expected quality after the mulligan is higher than your current score of 0.5.

---

**👤 You:**
> "Show me the full probability distribution for drawing targets from a 40-card deck with 4 copies of a card in my next 5 draws."

**🤖 AI Agent:**
> The distribution is: 0 targets: 56.5%, 1 target: 35.7%, 2 targets: 7.2%, 3 targets: 0.6%, 4 targets: 0.01%.


## ❓ FAQ

**Q: How does the calculator handle mulligans?**
The `evaluate_mulligan_decision` tool compares your current hand's quality score against the statistical expectation of a new hand, accounting for the reduction in hand size caused by the `mulliganPenalty`.

**Q: Can I track changes to my deck after scrying?**
Yes, use the `track_deck_progression` tool to update your `currentDeckSize` and `currentTargetCount` after seeing cards via scry or removing cards through deck thinning.

**Q: What mathematical model is used for these calculations?**
The server uses the hypergeometric distribution, which is the standard model for sampling without replacement from a finite population, making it perfect for card games.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/card-draw-probability-calculator](https://vinkius.com/mcp/card-draw-probability-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Card Draw Probability Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `card-draw-probability-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Card Draw Probability Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "card-draw-probability-calculator": {
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
