# Workout Quality Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/workout-quality-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify and analyze the multidimensional quality of your training sessions.

## Description
This MCP server provides a comprehensive system to evaluate physical training performance through four core pillars: RPE, Volume, Technique, and Mental Focus. By using `get_workout_quality`, you can calculate a holistic quality score and identify specific improvement areas. You can also use `get_quality_trend` to track performance over time, `compare_session_to_baseline` to see how a session deviates from your norms, and `identify_bottlenecks` to isolate the primary factor dragging down your session quality.


## Available Tools (4)
- **compare_session_to_baseline**: Determine how a single session's performance deviates from the user's established norms
- **get_quality_trend**: Analyze how workout quality has changed over a specific period
- **get_workout_quality**: Calculate the holistic quality score and detailed breakdown for a specific workout session
- **identify_bottlenecks**: Isolate which specific pillar is most significantly dragging down the total quality index


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workout Quality Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my workout quality for a session with RPE 8, 5000kg volume, 90 technique score, and 85 focus score."

**🤖 AI Agent:**
> Your workout quality index is 88.5. Your technique and focus were excellent, effectively maximizing your volume.

---

**👤 You:**
> "How has my workout quality trended from 2024-01-01 to 2024-01-31?"

**🤖 AI Agent:**
> Your workout quality has shown an upward trend with an average quality of 78 and low volatility.

---

**👤 You:**
> "Compare my current quality index of 75 to my baseline of 80."

**🤖 AI Agent:**
> Your session was Below Baseline, with a deviation of -5 points.


## ❓ FAQ

**Q: How is the quality index calculated?**
The index is a composite value derived from RPE, volume, technique quality, and mental focus. High technique and focus scores act as multipliers for the effective volume.

**Q: Can I see how my training is progressing over time?**
Yes, you can use the `get_quality_trend` tool to analyze how your workout quality has changed over a specific date range.

**Q: What should I do if my quality score is low?**
You can use `identify_bottlenecks` to find the specific pillar--such as technique or focus--that is most significantly impacting your session quality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/workout-quality-index](https://vinkius.com/en/ai-agent-connect/workout-quality-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Workout Quality Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `workout-quality-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Workout Quality Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workout-quality-index": {
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
