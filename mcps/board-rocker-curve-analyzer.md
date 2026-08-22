# Board Rocker Curve Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/board-rocker-curve-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Calculate precise surfboard rocker curves and performance profiles.

## Description
This MCP server provides deterministic tools for surfboard shaping and design. Use `analyze_rocker_geometry` to calculate the parabolic equation ($y = ax^2 + bx + c$), mid-point rocker, and rocker ratio based on nose and tail measurements. You can also use `get_performance_profile` to categorize the board's intended use, such as Speed/Paddling, All-around, or Steep waves/Turns, and `validate_rocker_inputs` to ensure dimensions are realistic for manufacturing.


## Available Tools (3)
- **analyze_rocker_geometry**: Calculates the primary geometric attributes and the mathematical parabolic equation of the surfboard
- **get_performance_profile**: Identifies the intended surfboard category based on the calculated rocker arc
- **validate_rocker_inputs**: Checks if the provided physical dimensions are realistic for surfboard manufacturing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Board Rocker Curve Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the rocker geometry for a 6ft surfboard with 2 inches of nose rocker and 1.5 inches of tail rocker."

**🤖 AI Agent:**
> The parabolic equation is $y = -0.0012x^2 + 0.015x + 1.75$, the mid-point rocker is 2.0 inches, the total rocker arc is 3.5 inches, the rocker ratio is 0.058, and the performance profile is All-around.

---

**👤 You:**
> "What is the performance profile for a board with a total rocker arc of 2 inches?"

**🤖 AI Agent:**
> A board with a 2-inch total rocker arc has a Speed/Paddling performance profile.

---

**👤 You:**
> "Check if a 100-inch board with 10 inches of nose rocker and 10 inches of tail rocker is valid."

**🤖 AI Agent:**
> The dimensions are invalid as the total rocker arc exceeds the maximum allowable percentage for a board of this length.


## ❓ FAQ

**Q: How do I calculate the parabolic equation for my board?**
You can use the `analyze_rocker_geometry` tool. Provide the board length, nose rocker, and tail rocker to receive the exact $y = ax^2 + bx + c$ equation.

**Q: What determines the performance profile of a surfboard?**
The performance profile is determined by the total rocker arc. The `get_performance_profile` tool categorizes boards into Speed/Paddling, All-around, or Steep waves/Turns based on this arc.

**Q: Can I validate if my rocker measurements are realistic?**
Yes, the `validate_rocker_inputs` tool checks if your provided nose and tail rocker measurements are within standard industry bounds for the given board length.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/board-rocker-curve-analyzer](https://vinkius.com/ai-agent-connect/board-rocker-curve-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Board Rocker Curve Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `board-rocker-curve-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Board Rocker Curve Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "board-rocker-curve-analyzer": {
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
