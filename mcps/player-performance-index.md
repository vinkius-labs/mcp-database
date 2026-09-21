# Player Performance Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/player-performance-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate deterministic football player performance scores using weighted statistical components.

## Description
This MCP server provides a deterministic engine to calculate standardized football player performance scores. By normalizing raw statistics like goals, assists, and tackles, and applying role-specific weights, it generates a precise index. The engine uses `calculate_player_index` to provide a full breakdown of contributions and `scale_by_efficiency` to adjust scores to a standard per-90-minutes basis, ensuring fair comparison between players with different playing times.


## Available Tools (4)
- **calculate_player_index**: Calculates the final performance index and provides a detailed breakdown
- **get_weight_configuration**: g., Attacker, Midfielder, Defender)

Retrieves the standard weight profiles for different player roles
- **scale_by_efficiency**: Adjusts a raw accumulated score to account for the duration of play
- **validate_component_ranges**: Checks if the provided statistics fall within the acceptable thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Player Performance Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the performance index for a player with 2 goals, 1 assist, 3 key passes, 2 tackles, 1 interception, 0 errors, and 90 minutes played, using Attacker weights."

**🤖 AI Agent:**
> The calculated performance index is 15.45 with a breakdown of goals: 0.8, assists: 0.4, key passes: 0.3, tackles: 0.1, and interceptions: 0.05.

---

**👤 You:**
> "What are the standard weights for a Defender role?"

**🤖 AI Agent:**
> The Defender profile weights are: goalWeight: 0.1, assistWeight: 0.1, keyPassWeight: 0.1, tackleWeight: 0.4, interceptionWeight: 0.3, and errorWeight: -0.2.

---

**👤 You:**
> "Adjust a raw score of 10.0 for a player who played only 45 minutes."

**🤖 AI Agent:**
> The efficiency-adjusted score for 45 minutes played is 20.0.


## ❓ FAQ

**Q: How is the performance score calculated?**
The score is calculated by normalizing raw statistics, applying weights defined by player roles, and then scaling the result based on minutes played using `scale_by_efficiency`.

**Q: Can I use different weights for different player roles?**
Yes, you can use `get_weight_configuration` to retrieve standard weight profiles for roles like Attacker, Midfielder, or Defender.

**Q: What happens if a player's stats are outside the normal range?**
You can use `validate_component_ranges` to check if statistics are within acceptable thresholds before performing calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/player-performance-index](https://vinkius.com/en/ai-agent-connect/player-performance-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Player Performance Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `player-performance-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Player Performance Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "player-performance-index": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
