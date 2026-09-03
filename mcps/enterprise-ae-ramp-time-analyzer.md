# Enterprise AE Ramp Time Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-ae-ramp-time-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Models and calculates Account Executive ramp progression, quota attainment, and productivity velocity.

## Description
This MCP server provides analytical tools to model the progression of Account Executives from onboarding to full productivity. It calculates essential sales metrics including average ramp duration, quota attainment trajectories, and milestone velocity. By accounting for factors like `dealComplexityFactor` and `territoryMaturityScore`, it provides a realistic view of sales performance. Use `calculate_average_ramp_metrics` for core summaries, `generate_ramp_curve` to visualize attainment over time, `project_attainment_trajectory` for revenue forecasting, and `evaluate_milestone_velocity` to track onboarding speed.


## Available Tools (4)
- **evaluate_milestone_velocity**: Measures how quickly an AE is moving through their onboarding stages
- **generate_ramp_curve**: Projects the expected percentage of quota attainment over a specific timeline
- **project_attainment_trajectory**: Forecasts future revenue/quota performance based on current progress
- **calculate_average_ramp_metrics**: Provides the core summary of an AE's expected time to full productivity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise AE Ramp Time Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the average ramp metrics for an AE with 3 months to first deal, 12 months to full quota, 40 training hours, a complexity of 1.2, and a maturity score of 0.8."

**🤖 AI Agent:**
> The average ramp duration is 13.4 months with a total productivity score of 85.

---

**👤 You:**
> "What is the projected revenue for an AE in month 6 who has achieved 40% quota, with a target of 12 months to full quota?"

**🤖 AI Agent:**
> The projected yearly revenue is $450,000 with an expected full attainment in month 12.

---

**👤 You:**
> "Check the onboarding velocity for an AE with 20 training hours, 3 milestones completed, and 2 months to first deal."

**🤖 AI Agent:**
> The velocity score is 75, indicating a healthy onboarding pace.


## ❓ FAQ

**Q: How does deal complexity affect the results?**
Higher complexity increases the expected ramp duration and flattens the attainment curve.

**Q: Can I forecast future revenue?**
Yes, you can use the trajectory tool to project future revenue based on current progress.

**Q: What inputs are needed for the ramp summary?**
You need time to first deal, time to full quota, training hours, complexity factor, and territory maturity score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-ae-ramp-time-analyzer](https://vinkius.com/ai-agent-connect/enterprise-ae-ramp-time-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise AE Ramp Time Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-ae-ramp-time-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise AE Ramp Time Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-ae-ramp-time-analyzer": {
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
