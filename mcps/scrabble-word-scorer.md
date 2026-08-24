# Scrabble Word Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/scrabble-word-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

A deterministic calculator for exact Scrabble scores, including multipliers and bingo bonuses.

## Description
This MCP server provides precise scoring for Scrabble moves. It calculates the base score of a word, applies letter multipliers (like Double Letter Score) to specific tiles, applies word multipliers (like Triple Word Score) to the total, and adds the 50-point bingo bonus if all seven tiles are used. Use `score_word` to calculate totals, `validate_rack` to ensure your tiles follow standard English distribution, and `get_standard_distribution` to reference official letter values.


## Available Tools (3)
- **get_standard_distribution**: Provides the authoritative reference for the standard English Scrabble letter counts and values
- **score_word**: Calculates the total score for a single word played on the board
- **validate_rack**: Checks if a set of tiles is valid according to standard English Scrabble rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scrabble Word Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the score for the word 'QUIZ' with a Double Letter Score on the 'Z'?"

**🤖 AI Agent:**
> The total score for 'QUIZ' is 22. (Q=10, U=1, I=1, Z=10. The 'Z' is doubled to 20, making the sum 10+1+1+20 = 32... wait, let me recalculate: Q(10)+U(1)+I(1)+Z(10*2=20) = 32. Total score is 32.)

---

**👤 You:**
> "Calculate the score for 'AXES' with a Triple Word Score."

**🤖 AI Agent:**
> The total score for 'AXES' is 24. (A=1, X=8, E=1, S=1. Sum is 11. 11 multiplied by 3 for the Triple Word Score equals 33. Wait, recalculating: 1+8+1+1 = 11. 11 * 3 = 33. The total score is 33.)

---

**👤 You:**
> "What is the score for 'QUARTZ' if I use all 7 tiles and there is a Double Word Score?"

**🤖 AI Agent:**
> The total score for 'QUARTZ' with a bingo bonus and a Double Word Score is 110. (Q=10, U=1, A=1, R=1, T=1, Z=10. Sum is 24. 24 * 2 for Double Word is 48. 48 + 50 bingo bonus = 98. Let me re-verify: 10+1+1+1+1+10 = 24. 24*2=48. 48+50=98. The total score is 98.)


## ❓ FAQ

**Q: How are multipliers applied?**
Letter multipliers are applied to individual tiles first. Once the sum of those tiles is calculated, the word multipliers are applied to that resulting sum.

**Q: What is a bingo bonus?**
A bingo bonus is a 50-point addition to the total score when a player uses all seven tiles from their rack in a single turn.

**Q: Can I check if my tiles are valid?**
Yes, you can use the `validate_rack` tool to check if your set of tiles adheres to the standard English Scrabble distribution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/scrabble-word-scorer](https://vinkius.com/ai-agent-connect/scrabble-word-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scrabble Word Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scrabble-word-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scrabble Word Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scrabble-word-scorer": {
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
