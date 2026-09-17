# Muscle Group Split Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/muscle-group-split-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates optimized weekly training schedules based on your recovery and goals.

## Description
This MCP server provides specialized tools to design personalized training architectures. Use `calculate_optimal_split` to determine the best split type (like PPL or Upper/Lower) based on your training frequency and recovery capacity. Once the architecture is set, `generate_volume_distribution` calculates the ideal weekly set counts for each muscle group. You can then use `plan_weekly_schedule` to map these sessions into a 7-day calendar, and `verify_recovery_viability` to ensure your proposed volume is safe and sustainable for your physiological limits.


## Available Tools (4)
- **calculate_optimal_split**: Determines the most effective training architecture for a user's specific constraints
- **generate_volume_distribution**: Calculates how much work (sets) should be allocated to different muscle groups
- **plan_weekly_schedule**: Maps the split and volume into a logical 7-day calendar
- **verify_recovery_viability**: An audit tool to ensure a proposed split does not violate biological recovery constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Muscle Group Split Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I can train 4 days a week, I have moderate recovery, and my goal is hypertrophy. What split should I use?"

**🤖 AI Agent:**
> For a 4-day frequency with moderate recovery and a hypertrophy goal, an Upper/Lower split is recommended to balance volume and frequency.

---

**👤 You:**
> "Generate a weekly schedule for a 3-day PPL split."

**🤖 AI Agent:**
> Monday: Push, Wednesday: Pull, Friday: Legs. Tuesday, Thursday, Saturday, and Sunday are recovery days.

---

**👤 You:**
> "How many sets should I do for chest if I'm doing a hypertrophy goal with high recovery?"

**🤖 AI Agent:**
> With high recovery capacity and a hypertrophy goal, you can sustain a higher weekly volume, typically ranging from 15 to 25 sets for the chest.


## ❓ FAQ

**Q: How do I know which split is best for me?**
You can use the `calculate_optimal_split` tool. It analyzes your training frequency, recovery capacity, and fitness goals to recommend the most effective architecture.

**Q: Can I check if my workout volume is too high?**
Yes, the `verify_recovery_viability` tool audits your proposed volume distribution against your recovery capacity to ensure safety.

**Q: Does this work with my existing training routine?**
The tools are designed to build a plan from your specific constraints, such as available days and recovery capacity, making it highly adaptable to your current lifestyle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/muscle-group-split-planner](https://vinkius.com/en/ai-agent-connect/muscle-group-split-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Muscle Group Split Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `muscle-group-split-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Muscle Group Split Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "muscle-group-split-planner": {
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
