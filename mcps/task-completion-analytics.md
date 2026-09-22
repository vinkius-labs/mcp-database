# Task Completion Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/task-completion-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate task completion percentages and productivity tiers.

## Description
This MCP server provides precise analytics for tracking workload progress. It allows AI agents to calculate raw completion percentages using `get_completion_percentage`, assign qualitative performance tiers via `get_completion_tier`, and generate comprehensive status reports with `get_workload_summary`. Additionally, it evaluates productivity against specific goals using `get_efficiency_metrics` to determine if targets are being met.


## Available Tools (4)
- **get_completion_percentage**: Calculates the raw percentage of completed tasks relative to the total workload
- **get_completion_tier**: Assigns a qualitative performance label based on the calculated completion percentage
- **get_efficiency_metrics**: Evaluates how effective the completion is by comparing the current progress against specific throughput targets
- **get_workload_summary**: Provides a high-level overview of task progress and productivity status for a specific workload


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Task Completion Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my completion percentage if I have finished 5 tasks out of 10?"

**🤖 AI Agent:**
> Your completion percentage is 50%.

---

**👤 You:**
> "Give me a summary of my progress: 8 tasks completed out of 10."

**🤖 AI Agent:**
> Your current progress is 80%, which falls into the High tier.

---

**👤 You:**
> "I have completed 7 tasks out of 10. Did I meet my 75% target?"

**🤖 AI Agent:**
> No, your current completion is 70%, which is 5% below your target of 75%.


## ❓ FAQ

**Q: How do I calculate my current progress?**
You can use the `get_completion_percentage` tool by providing the number of completed tasks and the total number of tasks.

**Q: What are the different performance tiers?**
The `get_completion_tier` tool categorizes progress into Low, Moderate, High, or Exceptional tiers based on the percentage achieved.

**Q: Can I check if I have met my productivity goal?**
Yes, use `get_efficiency_metrics` with your target percentage to see if your current progress meets or exceeds your goal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/task-completion-analytics](https://vinkius.com/en/ai-agent-connect/task-completion-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Task Completion Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `task-completion-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Task Completion Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "task-completion-analytics": {
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
