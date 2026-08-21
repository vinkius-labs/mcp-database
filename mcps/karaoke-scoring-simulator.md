# Karaoke Scoring Simulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/karaoke-scoring-simulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [entertainment](../categories/entertainment.md)

A deterministic simulator for Japanese karaoke scoring (DAM/JOYSOUND) based on pitch, rhythm, and vibrato.

## Description
This MCP server provides a precise simulation of professional Japanese karaoke scoring systems like DAM and JOYSOUND. It allows AI agents to evaluate singing performance by calculating deductions for pitch and rhythm errors, applying technical bonuses for vibrato, and scaling the final result based on song difficulty. Use `score_performance` to get a complete breakdown of metrics, or `validate_performance_inputs` to ensure singer data is within valid ranges before processing.


## Available Tools (3)
- **get_difficulty_multiplier**: Retrieves the scaling factor associated with a specific song difficulty level
- **score_performance**: Calculates the final performance metrics and score based on singer accuracy and song difficulty
- **validate_performance_inputs**: Checks if a set of performance metrics is mathematically valid before processing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Karaoke Scoring Simulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the score for a singer with 90% pitch accuracy, 85% rhythm accuracy, 4 vibrato instances, and a song difficulty of 3."

**🤖 AI Agent:**
> The performance results are: pitch deduction of 5.0, rhythm deduction of 4.5, vibrato bonus of 2.0, and a final score of 93.

---

**👤 You:**
> "What is the difficulty multiplier for a song with difficulty level 5?"

**🤖 AI Agent:**
> The multiplier for difficulty level 5 is 1.1.

---

**👤 You:**
> "Check if these metrics are valid: pitch 105%, rhythm 90%, vibrato 2, difficulty 3."

**🤖 AI Agent:**
> The metrics are invalid. The pitch accuracy percentage must be between 0 and 100.


## ❓ FAQ

**Q: How is the final score calculated?**
The score starts at 100, subtracts deductions for pitch and rhythm accuracy, adds a vibrato bonus (up to 10), and applies a multiplier based on the song difficulty level.

**Q: Can I validate my input data first?**
Yes, you can use the `validate_performance_inputs` tool to check if the pitch, rhythm, vibrato, and difficulty values are within the required mathematical ranges.

**Q: What is the maximum vibrato bonus?**
The vibrato bonus is calculated as the number of vibrato instances multiplied by 0.5, with a maximum possible bonus of 10.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/karaoke-scoring-simulator](https://vinkius.com/ai-agent-connect/karaoke-scoring-simulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Karaoke Scoring Simulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `karaoke-scoring-simulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Karaoke Scoring Simulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "karaoke-scoring-simulator": {
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
