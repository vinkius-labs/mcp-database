# Bowling Score Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bowling-score-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Deterministic 10-pin bowling scoring and validation engine.

## Description
This MCP server provides a professional-grade engine for calculating 10-pin bowling scores. It allows AI agents to process roll sequences to determine cumulative frame scores, total game scores, strike and spare counts, and identify special achievements like a Turkey or a Perfect Game. Use `calculate_game_score` to get a full scoring profile, `validate_roll_sequence` to check for rule violations, or `get_frame_statistics` for deep analysis of a specific frame.


## Available Tools (3)
- **calculate_game_score**: Calculates the complete scoring profile for a single game of bowling
- **get_frame_statistics**: Provides detailed analytical data for a specific frame within a game
- **validate_roll_sequence**: Checks if a provided sequence of rolls adheres to the fundamental rules of 10-pin bowling


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bowling Score Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the score for this bowling game: X, 7, /, 9, 0, X, X, X, X, X, X, X"

**🤖 AI Agent:**
> The total score is 133. The game included 10 strikes and 1 spare.

---

**👤 You:**
> "Is the sequence ['X', '11'] a valid bowling game?"

**🤖 AI Agent:**
> No, the sequence is invalid. Violation: Excessive pins in frame 1.

---

**👤 You:**
> "What are the statistics for frame 1 in the sequence ['X', '7', '/', '9', '0']?"

**🤖 AI Agent:**
> Frame 1 was a Strike with 10 pins knocked down and a cumulative score of 10.


## ❓ FAQ

**Q: How do I calculate the total score for a game?**
You can use the `calculate_game_score` tool by providing an array of rolls (e.g., ['X', '7', '/', '9', '0']). It will return the total score along with frame-by-frame details.

**Q: Can this engine detect a perfect game?**
Yes, the `calculate_game_score` tool includes an `isPerfectGame` boolean which returns true if the sequence represents 12 consecutive strikes.

**Q: How can I check if a bowling sequence is legal?**
Use the `validate_roll_sequence` tool. It will return whether the sequence is valid and provide a list of specific violations if any rules were broken.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bowling-score-engine](https://vinkius.com/ai-agent-connect/bowling-score-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bowling Score Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bowling-score-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bowling Score Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bowling-score-engine": {
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
