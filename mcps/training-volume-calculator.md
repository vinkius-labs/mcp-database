# Training Volume Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/training-volume-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Quantify training workload, muscle distribution, and intensity metrics.

## Description
This MCP server provides advanced analytical tools for strength athletes to track training progress. Use `calculate_session_metrics` to get a snapshot of total volume load and muscle group distribution for a single session. Use `analyze_muscle_balance` to evaluate physiological balance across muscle groups, `get_weekly_trends` to monitor progressive overload over time, and `calculate_intensity_profile` to determine the difficulty of training blocks using load and tempo data.


## Available Tools (4)
- **analyze_muscle_balance**: Analyze muscle balance
- **calculate_intensity_profile**: Calculate intensity profile
- **calculate_session_metrics**: Calculate session metrics
- **get_weekly_trends**: Get weekly trends


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Training Volume Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the metrics for my session: I did 3 sets of 10 reps at 100kg for Bench Press (Chest) and 4 sets of 12 reps at 80kg for Squats (Legs)."

**🤖 AI Agent:**
> Your total volume load for this session is 5,200kg, with 3,000kg allocated to Chest and 3,840kg to Legs.

---

**👤 You:**
> "Am I training my muscles evenly based on my last 3 sessions?"

**🤖 AI Agent:**
> Your training is currently imbalanced, with a high focus on Back volume compared to Chest volume.

---

**👤 You:**
> "What is my volume trend for the last month?"

**🤖 AI Agent:**
> Your weekly volume load has increased by 5% each week over the last month, indicating steady progressive overload.


## ❓ FAQ

**Q: How do I calculate my session metrics?**
You can use the `calculate_session_metrics` tool by providing a JSON array of your exercises, including sets, reps, and weight.

**Q: Can I track my progress over several weeks?**
Yes, the `get_weekly_trends` tool allows you to track volume load and time under tension progression over multiple weeks.

**Q: How is muscle balance determined?**
The `analyze_muscle_balance` tool compares your volume load across different muscle groups to identify imbalances.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/training-volume-calculator](https://vinkius.com/en/ai-agent-connect/training-volume-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Training Volume Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `training-volume-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Training Volume Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "training-volume-calculator": {
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
