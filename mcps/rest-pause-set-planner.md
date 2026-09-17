# Rest-Pause Set Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rest-pause-set-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates optimized rest-pause training protocols and fatigue projections.

## Description
This MCP server provides specialized tools for high-intensity hypertrophy training. It allows AI agents to calculate precise rest-pause protocols, including mini-set breakdowns and rest intervals. Users can use `get_protocol_plan` to generate a step-by-step execution plan, `get_fatigue_projection` to estimate recovery needs, `validate_session_feasibility` to check if a volume goal is realistic, and `get_volume_summary` to analyze total work performed.


## Available Tools (4)
- **get_fatigue_projection**: 
- **get_protocol_plan**: 
- **get_volume_summary**: 
- **validate_session_feasibility**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rest-Pause Set Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a rest-pause set for 100kg where I can do 8 reps before failure, with 20 seconds rest, aiming for 15 total reps."

**🤖 AI Agent:**
> Your rest-pause protocol is: Set 1: 8 reps, Set 2: 4 reps, Set 3: 3 reps. Total reps: 15. Total rest time: 40 seconds.

---

**👤 You:**
> "Is it feasible to hit 25 reps if my failure reps are 10?"

**🤖 AI Agent:**
> No, a goal of 25 reps is likely infeasible as it exceeds the biological limits for rest-pause training at your current capacity.

---

**👤 You:**
> "What was my total volume for a set of 8, 5, and 3 reps at 100kg?"

**🤖 AI Agent:**
> The total volume performed is 1600kg, with an average of 5.33 reps per set.


## ❓ FAQ

**Q: How do I generate a training plan?**
You can use the `get_protocol_plan` tool by providing your starting weight, failure reps, rest duration, and target goal reps.

**Q: Can I check if my training goal is too ambitious?**
Yes, use the `validate_session_feasibility` tool to determine if your desired volume is biologically realistic based on your current capacity.

**Q: How much recovery time do I need?**
The `get_fatigue_projection` tool estimates your recovery hours based on the intensity and volume of your planned protocol.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rest-pause-set-planner](https://vinkius.com/en/ai-agent-connect/rest-pause-set-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rest-Pause Set Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rest-pause-set-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rest-Pause Set Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rest-pause-set-planner": {
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
