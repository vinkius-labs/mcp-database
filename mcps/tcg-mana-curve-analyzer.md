# TCG Mana Curve Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tcg-mana-curve-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

A deterministic probability engine for TCG deckbuilding and mana consistency.

## Description
This MCP server provides a deterministic probability engine for Trading Card Game (TCG) deckbuilders. It uses hypergeometric distribution to calculate the likelihood of drawing specific cards or lands in an opening hand. Use `analyze_opening_hand` to check your starting hand reliability, `evaluate_mana_consistency` to assess land drops on turns 1 through 4, and `optimize_land_count` to find the ideal resource count based on your average mana value and mulligan rules.


## Available Tools (3)
- **analyze_opening_hand**: Calculate the probability of drawing specific cards or lands in the opening 7-card hand
- **evaluate_mana_consistency**: Evaluate the reliability of hitting land drops on turns 1 through 4
- **optimize_land_count**: Determine the ideal number of lands to include based on CMC and Mulligan rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TCG Mana Curve Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the probability of drawing at least one copy of a 4-of card in a 60-card deck with a 7-card opening hand?"

**🤖 AI Agent:**
> The probability of drawing at least one copy of that card in your opening 7 is approximately 40.2%.

---

**👤 You:**
> "How consistent is my 60-card deck with 24 lands for hitting land drops on turn 3?"

**🤖 AI Agent:**
> With 24 lands in a 60-card deck, you have a 72.4% probability of having enough lands to hit your 3rd land drop.

---

**👤 You:**
> "What is the optimal land count for a 60-card deck with an average mana value of 3.2 using London Mulligan?"

**🤖 AI Agent:**
> The optimal land count for your deck is 26 lands, providing a high stability score for your mana curve.


## ❓ FAQ

**Q: How does the engine calculate probabilities?**
The engine uses the hypergeometric distribution to calculate the probability of successes in a sequence of draws from a finite population without replacement.

**Q: Can I simulate different mulligan rules?**
Yes, the `optimize_land_count` tool allows you to simulate different rules, such as the London Mulligan.

**Q: What is the purpose of the mana consistency tool?**
The `evaluate_mana_consistency` tool assesses how reliable your deck is at hitting land drops on turns 1 through 4.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tcg-mana-curve-analyzer](https://vinkius.com/ai-agent-connect/tcg-mana-curve-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TCG Mana Curve Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tcg-mana-curve-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TCG Mana Curve Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tcg-mana-curve-analyzer": {
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
