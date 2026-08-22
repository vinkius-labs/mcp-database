# Enemy Difficulty Curve Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enemy-difficulty-curve-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze enemy scaling and player progression to ensure smooth combat pacing.

## Description
This MCP server provides deterministic diagnostic tools for game designers to identify friction points in combat progression. Use `analyze_combat_ratios` to calculate the relationship between enemy threat and player power, `detect_progression_anomalies` to find difficulty spikes and smoothness scores, and `evaluate_player_experience` to quantify frustration and boss impact. It helps ensure that difficulty curves remain engaging rather than frustrating or boring.


## Available Tools (3)
- **analyze_combat_ratios**: Calculates the fundamental relationship between enemy threat and player power
- **detect_progression_anomalies**: Identifies problematic jumps in difficulty and assesses the overall smoothness of the game flow
- **evaluate_player_experience**: Quantifies the qualitative "feel" of the game, specifically looking for boredom and frustration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enemy Difficulty Curve Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the combat ratios for these enemies: [{'level': 1, 'hp': 100, 'damage': 10, 'abilities_count': 1, 'special_mechanics': []}, {'level': 2, 'hp': 250, 'damage': 25, 'abilities_count': 2, 'special_mechanics': []}] with a player DPS curve of [10, 20]."

**🤖 AI Agent:**
> { "difficulty_ratios": [1.0, 1.25], "time_to_kill_per_enemy": [10.0, 10.0] }

---

**👤 You:**
> "Check for progression anomalies in these difficulty ratios: [1.0, 1.2, 2.5, 2.6]."

**🤖 AI Agent:**
> { "smoothness_score": 65.4, "spike_locations": [2], "is_unstable": true }

---

**👤 You:**
> "Evaluate the player experience with TTK values [15, 70, 20] and boss ratios [4.0]."

**🤖 AI Agent:**
> { "frustration_index": 1, "progression_pace": [1], "boss_ratios_valid": true }


## ❓ FAQ

**Q: How do I identify a difficulty spike?**
A difficulty spike is identified when the difficulty ratio increases by more than 50% compared to the previous enemy. You can use `detect_progression_anomalies` to find these specific locations.

**Q: What is a good Boss Ratio?**
A boss ratio is considered valid and well-tuned if the boss difficulty is between 3 and 5 times the average difficulty of the surrounding minion enemies.

**Q: How is the frustration index calculated?**
The frustration index counts the number of encounters where the time to kill (TTK) exceeds 60 seconds, indicating potentially tedious combat.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enemy-difficulty-curve-analyzer](https://vinkius.com/ai-agent-connect/enemy-difficulty-curve-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enemy Difficulty Curve Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enemy-difficulty-curve-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enemy Difficulty Curve Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enemy-difficulty-curve-analyzer": {
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
