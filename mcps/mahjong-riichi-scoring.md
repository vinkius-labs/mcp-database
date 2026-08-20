# Mahjong Riichi Scoring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mahjong-riichi-scoring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Deterministic Japanese Riichi Mahjong scoring calculator.

## Description
This MCP server provides precise scoring calculations for Japanese Riichi Mahjong. It handles the complex logic of converting han and fu into total points, applying scoring plateaus like Mangan and Yakuman, and determining exact payout distributions for both Ron and Tsumo wins. Use `calculate_final_score` to get the complete breakdown of points gained and lost, or `calculate_score_tier` to identify the specific scoring plateau of a hand.


## Available Tools (3)
- **calculate_final_score**: The primary entry point to calculate the total points gained by the winner and the distribution of losses
- **calculate_score_tier**: Identifies which scoring plateau (Mangan, Haneman, etc.) a hand falls into
- **get_payout_distribution**: Determines exactly how many points each player must pay based on the win type and dealer status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mahjong Riichi Scoring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the score for a hand with 4 han and 30 fu where the winner is the dealer and it was a Ron win."

**🤖 AI Agent:**
> The total points gained is 8000.

---

**👤 You:**
> "What is the scoring tier for 1 han and 20 fu?"

**🤖 AI Agent:**
> The hand falls into the standard scoring tier.

---

**👤 You:**
> "Calculate the payout for a Tsumo win with 2 han and 40 fu where the winner is not the dealer."

**🤖 AI Agent:**
> The winner receives 2000 points, with the dealer paying 1000 and the other two players paying 500 each.


## ❓ FAQ

**Q: How does the scoring handle dealer status?**
The tool accounts for dealer status in the `get_payout_distribution` logic, ensuring that in a Tsumo win, the dealer pays a different amount than non-dealers.

**Q: What are the scoring plateaus?**
The server implements standard Riichi plateaus including Mangan, Haneman, Baiman, Sanbaiman, and Yakuman via the `calculate_score_tier` tool.

**Q: Can I calculate the exact points for a specific hand?**
Yes, by using the `calculate_final_score` tool with the number of han, fu, dealer status, and win type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mahjong-riichi-scoring](https://vinkius.com/ai-agent-connect/mahjong-riichi-scoring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mahjong Riichi Scoring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mahjong-riichi-scoring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mahjong Riichi Scoring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mahjong-riichi-scoring": {
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
