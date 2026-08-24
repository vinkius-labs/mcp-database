# Mahjong Scoring Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mahjong-scoring-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

A deterministic Riichi Mahjong scoring calculator for Yaku, Fu, and final scores.

## Description
This MCP server provides precise, deterministic scoring for Riichi Mahjong. It connects AI agents to the complex logic of Japanese Mahjong scoring, including Yaku identification, Fu calculation, and final score distribution. Use `calculate_hand_value` to find the total Han and specific Yaku, `calculate_fu_points` to determine the point base, and `calculate_final_score` to get the final payment breakdown for both Tsumo and Ron wins.


## Available Tools (3)
- **calculate_final_score**: Converts Han and Fu into the final score and payment breakdown
- **calculate_fu_points**: Calculates the Fu (point base) of the winning hand
- **calculate_hand_value**: Calculates the total Han count and lists applicable Yaku for a Mahjong hand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mahjong Scoring Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the hand value for these tiles: 123m 456p 789s 11z 234s, with no dora, no riichi, and it is a closed hand."

**🤖 AI Agent:**
> The total Han is 1 (Tanyao).

---

**👤 You:**
> "What is the final score for a 4 Han, 30 Fu hand where the winner is the dealer and it was a Ron win?"

**🤖 AI Agent:**
> The final score is 8000 points, paid by a single player.

---

**👤 You:**
> "Calculate the Fu for a hand with tiles 123m 456p 789s 11z 234s, winning tile 1z, win type tsumo, and the hand is closed."

**🤖 AI Agent:**
> The total Fu is 30.


## ❓ FAQ

**Q: How do I calculate the total Han?**
You can use the `calculate_hand_value` tool. Provide the 14 tiles, dora indicators, and whether the hand is open or closed.

**Q: Does this handle dealer multipliers?**
Yes, the `calculate_final_score` tool automatically applies the 1.5x multiplier for the dealer.

**Q: Can I calculate Fu for a Tsumo win?**
Yes, use `calculate_fu_points` and specify 'tsumo' as the win type to include the necessary Tsumo points.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mahjong-scoring-engine](https://vinkius.com/ai-agent-connect/mahjong-scoring-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mahjong Scoring Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mahjong-scoring-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mahjong Scoring Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mahjong-scoring-engine": {
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
