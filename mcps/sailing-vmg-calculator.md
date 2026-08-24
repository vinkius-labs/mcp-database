# Sailing VMG Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sailing-vmg-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Deterministic sailing vector math and performance calculator for wind and speed analysis.

## Description
This MCP server provides precise sailing vector mathematics to help sailors optimize their performance. It connects AI agents to critical sailing calculations including apparent wind determination via `calculate_apparent_wind`, efficiency analysis using `calculate_vmg_performance`, sideways drift prediction with `estimate_leeway`, and finding optimal headings through `get_optimal_angles`. It is designed to help navigate complex wind conditions by calculating Velocity Made Good (VMG) and leeway based on boat polar data.


## Available Tools (4)
- **calculate_apparent_wind**: Determine the wind conditions experienced on the vessel
- **calculate_vmg_performance**: Calculate the efficiency of the current heading relative to a target course
- **estimate_leeway**: Predict the sideways drift caused by wind pressure
- **get_optimal_angles**: Find the most efficient headings for upwind and downwind travel based on boat characteristics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sailing VMG Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my apparent wind if the true wind is 15 knots at 45 degrees and my boat speed is 6 knots?"

**🤖 AI Agent:**
> The apparent wind speed is 11.85 knots and the apparent wind angle is 32.4 degrees.

---

**👤 You:**
> "Calculate my VMG for a target course angle of 20 degrees with a true wind of 12 knots, boat speed of 5 knots, and true wind angle of 40 degrees."

**🤖 AI Agent:**
> Your Velocity Made Good (VMG) is 4.72 knots.

---

**👤 You:**
> "Estimate the leeway for a boat moving at 5 knots in 10 knots of true wind at a 30 degree angle."

**🤖 AI Agent:**
> The estimated leeway angle is 3.5 degrees.


## ❓ FAQ

**Q: How do I calculate my apparent wind?**
You can use the `calculate_apparent_wind` tool by providing the true wind speed, true wind angle, and your current boat speed.

**Q: Can I find my best sailing angles?**
Yes, the `get_optimal_angles` tool uses your boat's polar data to find the most efficient upwind and downwind headings.

**Q: What is VMG?**
Velocity Made Good (VMG) is the speed component in the direction of your target course. You can calculate this using `calculate_vmg_performance`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sailing-vmg-calculator](https://vinkius.com/ai-agent-connect/sailing-vmg-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sailing VMG Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sailing-vmg-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sailing VMG Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sailing-vmg-calculator": {
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
