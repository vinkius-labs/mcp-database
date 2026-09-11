# Mine Production Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mine-production-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimizes mine production schedules, cutoff grades, and NPV using linear programming.

## Description
This MCP server provides specialized tools for mining engineers to optimize production schedules. It connects AI agents to core mining optimization logic, allowing for the calculation of annual production timelines, optimal cutoff grades, and total project Net Present Value (NPV). Users can use `calculate_annual_production_schedule` to generate mining timelines, `determine_period_cutoff_grades` to find optimal grade thresholds, and `calculate_project_npv` to evaluate economic feasibility. Additionally, `validate_blending_constraints` ensures that the planned ore extraction meets specific material quality requirements.


## Available Tools (4)
- **calculate_annual_production_schedule**: Generates a high-level timeline of mining and processing activities
- **calculate_project_npv**: Calculates the total economic value of the proposed mining plan
- **determine_period_cutoff_grades**: Identifies the optimal grade threshold for each period to maximize value
- **validate_blending_constraints**: Checks if the planned production meets the necessary material quality specifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mine Production Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a production schedule for my block model with a processing capacity of 5000 tons and a mining capacity of 7000 tons."

**🤖 AI Agent:**
> The production schedule has been generated. In Period 0, 6500 tons were mined and 5000 tons were processed with an average ore grade of 0.45%.

---

**👤 You:**
> "What is the NPV for this mining plan given a metal price of $1500 and a discount rate of 10%?"

**🤖 AI Agent:**
> The total Net Present Value (NPV) for the proposed mining plan is $45,250,000, with total revenue of $120,000,000 and total costs of $74,750,000.

---

**👤 You:**
> "Calculate the optimal cutoff grades for the current production schedule with a metal price of $1200 and operating cost of $300."

**🤖 AI Agent:**
> The optimal cutoff grades for the periods are: Period 0: 0.32, Period 1: 0.35, and Period 2: 0.38.


## ❓ FAQ

**Q: How do I calculate the project's total value?**
You can use the `calculate_project_npv` tool, providing the production schedule, cutoff grades, and economic parameters like metal price and discount rate.

**Q: Can I check if my ore blending meets quality targets?**
Yes, the `validate_blending_constraints` tool checks if the planned production schedule complies with your specified target grades and allowed deviations.

**Q: What inputs are needed for the production schedule?**
To use `calculate_annual_production_schedule`, you need the block model data, the processing capacity limit, and the mining capacity limit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mine-production-scheduler](https://vinkius.com/en/ai-agent-connect/mine-production-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mine Production Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mine-production-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mine Production Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mine-production-scheduler": {
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
