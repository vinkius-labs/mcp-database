# Refinery Turnaround Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refinery-turnaround-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimize refinery turnaround schedules by analyzing critical paths, resource needs, and inspection impacts.

## Description
This MCP server provides specialized planning tools for refinery turnaround management. It allows AI agents to calculate the `get_critical_path` to identify scheduling bottlenecks, use `calculate_resource_requirements` to ensure contractor availability meets demand, and `estimate_turnaround_duration` to predict completion timelines. Additionally, it can `simulate_scope_expansion` to evaluate how unexpected inspection findings might delay the entire operation.


## Available Tools (4)
- **calculate_resource_requirements**: Estimates the total man-hours and equipment needs based on the scope
- **estimate_turnaround_duration**: Predicts the total time needed to complete the turnaround, accounting for potential inspection-driven delays
- **get_critical_path**: Identifies the sequence of tasks that dictates the total turnaround duration
- **simulate_scope_expansion**: Evaluates how the critical path and duration change when new inspection findings are added


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refinery Turnaround Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the critical path for my current maintenance scope and dependencies?"

**🤖 AI Agent:**
> The critical path consists of tasks T1, T4, and T7, with a total duration of 14 days. The bottleneck is task T4.

---

**👤 You:**
> "Will we have enough welders for this turnaround?"

**🤖 AI Agent:**
> No, there is a shortfall of 3 welders during the peak demand period in week 2.

---

**👤 You:**
> "Estimate the turnaround duration if we expect some extra inspection findings."

**🤖 AI Agent:**
> The estimated duration is 22 days, including a 4-day buffer for expected inspection findings.


## ❓ FAQ

**Q: How does the tool identify the critical path?**
The `get_critical_path` tool analyzes the sequence of dependent tasks to find the longest chain of activities that determines the total turnaround duration.

**Q: Can I simulate the impact of unexpected repairs?**
Yes, you can use `simulate_scope_expansion` to see how new inspection findings will change the critical path and increase the total duration.

**Q: How are resource shortages handled?**
The `calculate_resource_requirements` tool compares the required man-hours and equipment against provided contractor availability to identify specific resource shortfalls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refinery-turnaround-planner](https://vinkius.com/en/ai-agent-connect/refinery-turnaround-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refinery Turnaround Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refinery-turnaround-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refinery Turnaround Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refinery-turnaround-planner": {
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
