# Recovery Time Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recovery-time-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate estimated recovery duration and progressive weekly plans based on burnout levels and mitigation strategies.

## Description
The Recovery Time Planner is an estimation engine designed to help individuals navigate the process of returning from burnout. By inputting your current exhaustion level (on a scale of 1-10) and choosing a mitigation strategy, you can receive concrete projections for your recovery journey.

Key features include:
- `calculate_estimated_duration`: Predicts the total number of weeks required to reach a healthy baseline using strategies like sleep extension, total disconnection, or capacity adjustment.
- `generate_weekly_plan`: Provides a structured, week-by-week progressive plan that transitions from intensive intervention to maintenance phases.
- `evaluate_strategy_suitability`: Analyzes whether your chosen strategy is appropriate for your current burnout tier (Low, Medium, or High) to ensure the most effective path to recovery.

This tool acts as a bridge between recognizing exhaustion and implementing actionable structural changes.


## Available Tools (3)
- **calculate_estimated_duration**: Calculate estimated recovery weeks
- **evaluate_strategy_suitability**: Evaluate if a strategy is appropriate
- **generate_weekly_plan**: Generate a progressive recovery plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recovery Time Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am feeling very exhausted, around a level 5. How many weeks will I need if I use the total disconnection strategy?"

**🤖 AI Agent:**
> Based on a burnout level of 5 and the total disconnection strategy, your estimated recovery duration is 6 weeks with a confidence score of 0.85.

---

**👤 You:**
> "Generate a weekly plan for me. My burnout level is 3 and I want to focus on sleep extension."

**🤖 AI Agent:**
> Week 1: Increase sleep duration by 2 hours.
Week 2: Implement strict digital sunset at 9 PM.
Week 3: Maintain consistent wake-up times.

---

**👤 You:**
> "Is capacity adjustment a good idea for someone at level 8 burnout?"

**🤖 AI Agent:**
> Yes, capacity adjustment is highly recommended for high-tier burnout (level 8) as it addresses the structural causes of exhaustion.


## ❓ FAQ

**Q: How do I know which burnout level I am at?**
The tool uses a scale of 1 to 10, where 1 represents mild fatigue and 10 represents extreme clinical burnout. You should assess your current state of exhaustion and physical/mental depletion.

**Q: What are the available mitigation strategies?**
The three primary strategies are `sleep_extension` (focusing on biological rest), `total_disconnection` (mental detachment from work), and `capacity_adjustment` (structural reduction of workload).

**Q: Can I use the tool to plan for a specific vacation period?**
Yes, by using the `generate_weekly_plan` tool with the `total_disconnection` strategy, you can see how a period of time away from work should be structured to maximize recovery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recovery-time-planner](https://vinkius.com/mcp/recovery-time-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recovery Time Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recovery-time-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recovery Time Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recovery-time-planner": {
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
