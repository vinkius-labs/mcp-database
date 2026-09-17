# Reverse Pyramid Training Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reverse-pyramid-training-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Design precise Reverse Pyramid Training (RPT) protocols with automated weight and rep calculations.

## Description
This MCP server provides a specialized engine for designing Reverse Pyramid Training (RPT) protocols. It allows users to calculate high-intensity top sets and descending back-off sets based on their estimated 1RM. You can use `plan_rpt_session` to generate a complete single-session prescription, `calculate_progression_increment` to determine weight increases for future sessions, and `validate_exercise_suitability` to ensure your chosen lifts fit the RPT methodology. It also includes `generate_weekly_volume_summary` to track your total weekly workload.


## Available Tools (4)
- **generate_weekly_volume_summary**: Provides a high-level view of the total workload expected for a specific exercise over a full week
- **calculate_progression_increment**: Determines how much weight should be added to the protocol for the next training session
- **plan_rpt_session**: Generates a complete single-session training prescription for a specific exercise
- **validate_exercise_suitability**: Checks if a selected exercise is appropriate for a standard RPT protocol


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reverse Pyramid Training Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan an RPT session for Bench Press with a 100kg 1RM, performed 2 times per week."

**🤖 AI Agent:**
> Your Bench Press session: Top set of 90kg for 5 reps, followed by two back-off sets of 80kg for 8 reps and 70kg for 10 reps. Total volume: 2100kg.

---

**👤 You:**
> "Is the Bicep Curl suitable for RPT?"

**🤖 AI Agent:**
> No, Bicep Curls are isolation exercises and are generally considered unsuitable for the core RPT intensity structure which focuses on compound movements.

---

**👤 You:**
> "I just did a top set of 120kg. How much should I add next time if I am an intermediate lifter?"

**🤖 AI Agent:**
> For an intermediate lifter, the recommended increment is 2.5kg, making your next top set 122.5kg.


## ❓ FAQ

**Q: How do I plan a new workout session?**
You can use the `plan_rpt_session` tool by providing your estimated 1RM, the exercise name, and your weekly training frequency.

**Q: Can I use any exercise with this planner?**
Not all exercises are ideal for RPT. Use `validate_exercise_suitability` to check if a movement is appropriate for this high-intensity methodology.

**Q: How much weight should I add each week?**
The `calculate_progression_increment` tool determines the appropriate weight increase based on your current top set weight and your experience level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reverse-pyramid-training-planner](https://vinkius.com/en/ai-agent-connect/reverse-pyramid-training-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reverse Pyramid Training Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reverse-pyramid-training-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reverse Pyramid Training Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reverse-pyramid-training-planner": {
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
