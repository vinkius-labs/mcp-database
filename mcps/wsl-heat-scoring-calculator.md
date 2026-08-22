# WSL Heat Scoring Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wsl-heat-scoring-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate professional World Surf League heat scores and win probabilities.

## Description
This MCP server provides deterministic scoring logic for World Surf League (WSL) heats. It calculates total heat scores, average wave scores, and win feasibility based on specific heat formats like 3-wave, 5-wave, or unlimited. Use `calculate_heat_score` to determine the required score to beat an opponent and check if a win is still mathematically possible.


## Available Tools (3)
- **calculate_heat_score**: Calculates the total heat score, average wave score, and win feasibility based on a surfer's waves and the heat format
- **get_heat_format_metadata**: Retrieves the configuration rules (number of waves to discard) for a specific heat type
- **validate_wave_score**: Checks if a specific wave score adheres to professional surfing scoring standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WSL Heat Scoring Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the score for a 3-wave heat where the waves are 8.5, 7.0, and 4.0, against an opponent with 14.0."

**🤖 AI Agent:**
> The top two scores are 8.5 and 7.0, resulting in a total heat score of 15.5 and an average wave score of 7.75. You need 0.1 more than the opponent's score to win, but since your current score is already 15.5, you have already surpassed the opponent.

---

**👤 You:**
> "What is the metadata for a 5-wave heat format?"

**🤖 AI Agent:**
> For a 5-wave heat, the system will discard the 3 lowest waves and keep the 2 highest waves.

---

**👤 You:**
> "Is it possible to win a heat if I need 21.0 points?"

**🤖 AI Agent:**
> No, it is not possible to win as the maximum possible score is 20.0.


## ❓ FAQ

**Q: What heat types are supported?**
The server supports 3-wave, 5-wave, and unlimited heat formats.

**Q: How is the win possibility determined?**
The `calculate_heat_score` tool checks if the score needed to beat the opponent exceeds the maximum possible score of 20.0.

**Q: Can I validate individual wave scores?**
Yes, you can use the `validate_wave_score` tool to ensure a score is within the professional range of 0.1 to 10.0.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wsl-heat-scoring-calculator](https://vinkius.com/ai-agent-connect/wsl-heat-scoring-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WSL Heat Scoring Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wsl-heat-scoring-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WSL Heat Scoring Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wsl-heat-scoring-calculator": {
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
