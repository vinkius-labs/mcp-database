# OKR Progress Tracking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/okr-progress-tracking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate OKR progress, forecasts, and stretch assessments.

## Description
This MCP server provides a mathematical engine for measuring the health of Objectives and Key Results (OKRs). It allows AI agents to calculate weighted progress scores, generate confidence-adjusted completion forecasts, and perform stretch goal assessments. Use `calculate_objective_progress` to find total progress, `forecast_objective_completion` to predict end-of-period results, `assess_stretch_status` to determine if a goal is on track or at risk, and `evaluate_dependency_impact` to see how lagging dependencies affect your targets.


## Available Tools (4)
- **assess_stretch_status**: Assess if the objective is on track, at risk, a stretch, or failing
- **calculate_objective_progress**: Calculate the current total progress percentage of an Objective
- **evaluate_dependency_impact**: Evaluate the impact of a lagging dependency on a Key Result
- **forecast_objective_completion**: Forecast the projected progress at the end of the period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OKR Progress Tracking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current progress for my objective with these KRs: { id: 'kr1', weight: 60, currentValue: 5, targetValue: 10 }, { id: 'kr2', weight: 40, currentValue: 2, targetValue: 10 }?"

**🤖 AI Agent:**
> The total progress for your objective is 35%.

---

**👤 You:**
> "Based on 40% progress and 70% confidence, where will we be in 4 weeks if the total period is 12 weeks?"

**🤖 AI Agent:**
> The projected progress at the end of the period is 65%.

---

**👤 You:**
> "Is my objective on track if progress is 50% and the forecast is 70% with high confidence?"

**🤖 AI Agent:**
> The objective is currently marked as a stretch.


## ❓ FAQ

**Q: How is the total progress calculated?**
The total progress is a weighted average of all Key Results. Each KR's progress (current value divided by target) is multiplied by its assigned weight, and the sum of these values represents the total progress.

**Q: What does the forecast tool do?**
The `forecast_objective_completion` tool uses your current progress, the remaining time, and your subjective confidence level to predict where your progress will stand at the end of the OKR cycle.

**Q: Can I check if a dependency is blocking my progress?**
Yes, you can use `evaluate_dependency_impact` to determine how much a lagging dependency is slowing down a specific Key Result.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/okr-progress-tracking](https://vinkius.com/en/ai-agent-connect/okr-progress-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OKR Progress Tracking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `okr-progress-tracking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OKR Progress Tracking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "okr-progress-tracking": {
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
