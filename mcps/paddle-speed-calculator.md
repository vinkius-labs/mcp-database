# Paddle Speed Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paddle-speed-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Predict paddling speed, catch rates, and wave count potential for surfboards.

## Description
This MCP server provides specialized hydrodynamic analysis for surfers. By connecting your AI assistant to Vinkius Edge, you can use tools like `get_paddle_speed` to predict maximum achievable speeds, `get_catch_rate` to determine wave interception probability, and `get_wave_count_potential` to estimate session efficiency. It also includes `get_board_efficiency_score` to evaluate how well a specific board matches your physical fitness and technical skill.


## Available Tools (4)
- **get_board_efficiency_score**: Provides a single metric to evaluate how "user-friendly" a specific board is for a specific surfer
- **get_wave_count_potential**: Estimates the efficiency of a session by predicting how many waves can be caught before fatigue sets in
- **get_catch_rate**: Calculates how effectively a surfer can intercept and match the speed of a moving wave
- **get_paddle_speed**: Predicts the maximum achievable paddling speed for a specific surfboard and surfer combination


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paddle Speed Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my expected paddling speed with a 35L, 6.0ft, 20in board if I have high fitness and intermediate technique?"

**🤖 AI Agent:**
> Your expected paddling speed is 1.2 m/s with a high performance rating.

---

**👤 You:**
> "How many waves can I catch in a 60 minute session with a 50L board, high fitness, and advanced technique?"

**🤖 AI Agent:**
> You can expect to catch approximately 15 waves during your 60 minute session.

---

**👤 You:**
> "Calculate my catch rate for a steep wave (level 8) using a 40L board, medium fitness, and beginner technique."

**🤖 AI Agent:**
> Your catch probability is 0.45 with an acceleration factor of 1.1.


## ❓ FAQ

**Q: How accurate are the speed predictions?**
Predictions are based on hydrodynamic models accounting for board volume, length, width, and user-specific factors like fitness and technique.

**Q: Can I use this with Claude Desktop?**
Yes, you can connect this server to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.

**Q: What does the efficiency score represent?**
The `get_board_efficiency_score` tool provides a normalized metric indicating how well a board's buoyancy and dimensions align with your current physical conditioning and paddling proficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paddle-speed-calculator](https://vinkius.com/en/ai-agent-connect/paddle-speed-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paddle Speed Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paddle-speed-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paddle Speed Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paddle-speed-calculator": {
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
