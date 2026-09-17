# German Volume Training Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/german-volume-training-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates hyper-structured 10x10 training cycles based on GVT principles.

## Description
This MCP server provides specialized tools to orchestrate the German Volume Training (GVT) protocol. It allows AI agents to calculate precise working weights, recommend optimal movement tempos, and manage progression based on performance. Use `plan_gvt_cycle` to build a full training progression, `calculate_working_weight` to determine starting loads, `get_tempo_recommendation` for movement timing, and `evaluate_progression_readiness` to decide when to increase weight.


## Available Tools (4)
- **plan_gvt_cycle**: Generates a complete training progression based on muscle groups and exercises
- **calculate_working_weight**: Determines the starting load for the GVT protocol
- **evaluate_progression_readiness**: Determines if the user should increase their weight
- **get_tempo_recommendation**: Provides the specific movement timing (tempo) required for GVT


## 💬 Prompt Examples

Here are some examples of how you can interact with the **German Volume Training Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a GVT cycle for Chest and Back with Squats and Bench Press, training 2 times a week."

**🤖 AI Agent:**
> Your GVT cycle is ready. You will perform 10 sets of 10 reps for Squats and Bench Press, with a recovery period of 3 days between sessions.

---

**👤 You:**
> "What weight should I use if my 1RM for Bench Press is 100kg and I want 60% intensity?"

**🤖 AI Agent:**
> You should use 60kg for your 10x10 sets.

---

**👤 You:**
> "What is the recommended tempo for hypertrophy in GVT?"

**🤖 AI Agent:**
> For hypertrophy, a tempo of 4-0-2-0 is recommended to maximize time under tension during the eccentric phase.


## ❓ FAQ

**Q: How do I use this to plan my workouts?**
You can use `plan_gvt_cycle` to generate a complete training plan by providing your target muscle groups and chosen exercises.

**Q: How is the weight determined?**
The `calculate_working_weight` tool determines the starting load based on your estimated one-repetition maximum and a target intensity percentage.

**Q: When should I increase my training weight?**
Use `evaluate_progression_readiness` to check if you have successfully completed all 10 sets of 10 reps to determine if you are ready for more weight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/german-volume-training-planner](https://vinkius.com/en/ai-agent-connect/german-volume-training-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **German Volume Training Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `german-volume-training-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **German Volume Training Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "german-volume-training-planner": {
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
