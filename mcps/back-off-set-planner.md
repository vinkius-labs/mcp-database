# Back-off Set Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/back-off-set-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimizes back-off set parameters to balance muscle growth and fatigue.

## Description
This MCP server provides specialized strength training calculations to help athletes manage training volume. By using the `get_backoff_scheme` tool, you can determine the ideal weight and repetition ranges following a heavy top set. You can also use `optimize_backoff_plan` to automatically find the best set/rep configuration that hits your target volume while respecting your chosen fatigue management level. It is designed to bridge the gap between heavy intensity and effective hypertrophy volume.


## Available Tools (4)
- **calculate_volume_compliance**: Determines how much of the total volume goal is met by the proposed back-off sets
- **get_backoff_scheme**: Calculates the specific weight, reps, and set count for a back-off routine
- **get_fatigue_stimulus_profile**: Provides a qualitative analysis of the efficiency of the training prescription
- **optimize_backoff_plan**: Iteratively finds the best set/rep configuration to meet a specific volume goal while respecting fatigue constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Back-off Set Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I did a top set of 100kg for 5 reps. I want moderate fatigue management. What should my back-off sets look like?"

**🤖 AI Agent:**
> For a 100kg top set with moderate fatigue management, you should perform 3 sets of 8 repetitions at 80kg.

---

**👤 You:**
> "Help me plan a back-off routine. Top set: 150lbs for 3 reps. Target volume: 2000lbs. I want high fatigue management."

**🤖 AI Agent:**
> To reach your 2000lbs target with high fatigue management, it is recommended to perform 5 sets of 12 repetitions at 110lbs.

---

**👤 You:**
> "I did 80kg for 10 reps as my top set. I'm doing 3 sets of 8 at 60kg. Did I hit my 1500lb volume goal?"

**🤖 AI Agent:**
> No, your total volume achieved is 1520lbs, which actually exceeds your 1500lb goal.


## ❓ FAQ

**Q: How do I use this to plan my workout?**
You can provide your top set weight and reps to the `get_backoff_scheme` tool, or use `optimize_backoff_plan` to hit a specific volume goal.

**Q: What is fatigue management?**
It is a setting that adjusts the intensity of your back-off sets. High fatigue management uses lower weights to prioritize recovery, while low management keeps intensity higher.

**Q: Can I check if I met my volume target?**
Yes, the `calculate_volume_compliance` tool allows you to verify if your planned sets meet your total volume goal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/back-off-set-planner](https://vinkius.com/en/ai-agent-connect/back-off-set-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Back-off Set Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `back-off-set-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Back-off Set Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "back-off-set-planner": {
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
