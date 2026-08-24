# Billiards Cut Angle Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/billiards-cut-angle-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports](../categories/sports.md)

Deterministic geometry engine for precision pool and billiards shot mechanics.

## Description
This MCP server provides a deterministic geometry engine for precision pool and billiards shot mechanics. It allows AI agents to calculate exact aiming points using ghost ball geometry, determine tangent lines for stun shots, and predict friction-induced throw deviation. Additionally, it uses the diamond system to predict cue ball rebound angles and exit points after hitting a rail, accounting for applied English. Use `calculate_impact_geometry` to find the ideal aiming position, `estimate_throw_deviation` to account for friction, and `predict_rail_rebound` to plan rail shots.


## Available Tools (3)
- **calculate_impact_geometry**: Determines the precise aiming point and fundamental angles for a specific shot
- **estimate_throw_deviation**: Predicts how much friction will pull the object ball off its intended geometric path
- **predict_rail_rebound**: Uses the diamond system to predict the cue ball's path after hitting a cushion


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Billiards Cut Angle Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the impact geometry for a shot where the cue ball is at (10, 10), the object ball is at (20, 20), and the pocket is at (30, 10), with a ball radius of 2.85."

**🤖 AI Agent:**
> The ideal ghost ball position is at (15.94, 15.94) with a cut angle of 45.0 degrees and a tangent line angle of 45.0 degrees.

---

**👤 You:**
> "What is the estimated throw deviation for a cut angle of 30 degrees with a spin intensity of 0.5?"

**🤖 AI Agent:**
> The estimated angular deviation caused by friction is 1.25 degrees.

---

**👤 You:**
> "Predict the rail rebound for an entry angle of 45 degrees using 'right' spin with a strength of 0.8 and a diamond fraction of 0.5."

**🤖 AI Agent:**
> The predicted exit angle is 52.3 degrees and the exit point is at (45.2, 12.8).


## ❓ FAQ

**Q: How do I calculate the correct aiming point?**
You can use the `calculate_impact_geometry` tool. Provide the coordinates for the cue ball, object ball, and target pocket to receive the precise ghost ball position and cut angle.

**Q: Can this tool predict how spin affects a rail rebound?**
Yes, the `predict_rail_rebound` tool uses the diamond system to calculate the exit angle and exit point, factoring in the type and strength of English applied.

**Q: Does it account for friction-induced deviation?**
Yes, the `estimate_throw_deviation` tool predicts how much friction will pull the object ball off its geometric path based on the cut angle and spin intensity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/billiards-cut-angle-calculator](https://vinkius.com/ai-agent-connect/billiards-cut-angle-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Billiards Cut Angle Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `billiards-cut-angle-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Billiards Cut Angle Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "billiards-cut-angle-calculator": {
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
