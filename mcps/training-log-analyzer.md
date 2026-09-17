# Training Log Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/training-log-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Identify physiological patterns and performance trends in strength training logs.

## Description
This MCP server connects AI agents to your strength training data to provide actionable insights. It analyzes training history to detect plateaus, track volume trends, and suggest periodization strategies. Use `detect_performance_plateaus` to see if you are stuck, `get_volume_trends` to monitor workload, or `recommend_periodization` to plan your next training phase.


## Available Tools (4)
- **analyze_progress_trajectory**: Am I getting stronger or weaker over the long term?
- **detect_performance_plateaus**: Am I stuck and unable to make progress in my lifts?
- **get_volume_trends**: How has my total workload changed over time for a specific exercise?
- **recommend_periodization**: What should my training focus be in the next phase to optimize results?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Training Log Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Am I stuck and unable to make progress in my lifts?"

**🤖 AI Agent:**
> No, your performance is still trending upwards, though progress has slowed slightly in the last 3 sessions.

---

**👤 You:**
> "How has my total workload changed over time for Bench Press?"

**🤖 AI Agent:**
> Your total volume for Bench Press has increased by 12% over the last 30 days.

---

**👤 You:**
> "What should my training focus be in the next phase to optimize results?"

**🤖 AI Agent:**
> Based on your recent plateau, a Deload phase is recommended to allow for recovery before starting a new strength cycle.


## ❓ FAQ

**Q: How can I know if I am stuck in my progress?**
You can use the `detect_performance_plateaus` tool to analyze your recent sessions and identify if your strength has stagnated.

**Q: Can this tool help me plan my training cycles?**
Yes, the `recommend_periodization` tool provides specific phase recommendations like Deload or Hypertrophy based on your performance data.

**Q: How is volume calculated?**
Volume is calculated as the total weight lifted multiplied by the number of repetitions performed for each exercise.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/training-log-analyzer](https://vinkius.com/en/ai-agent-connect/training-log-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Training Log Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `training-log-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Training Log Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "training-log-analyzer": {
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
