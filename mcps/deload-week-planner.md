# Deload Week Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/deload-week-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate optimal recovery parameters and deload strategies for strength athletes.

## Description
This MCP server provides specialized tools for strength athletes to manage training fatigue. It calculates volume reduction, intensity maintenance, and recovery timelines using proactive or reactive deload methodologies. Use `plan_deload` to generate a full recovery strategy, `evaluate_fatigue_status` to check if immediate rest is needed, `get_exercise_templates` for movement adjustments, and `calculate_recovery_timeline` to estimate return-to-play dates.


## Available Tools (4)
- **evaluate_fatigue_status**: evaluate_fatigue_status
- **get_exercise_templates**: get_exercise_templates
- **plan_deload**: 
- **calculate_recovery_timeline**: calculate_recovery_timeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deload Week Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am in a strength phase, my fatigue is at 8/10, and my performance has been decreasing for 2 weeks. Should I deload?"

**🤖 AI Agent:**
> Yes, based on your decreasing performance and high fatigue, a reactive deload is recommended with a 40% volume reduction and 7-day duration.

---

**👤 You:**
> "Check my fatigue status. I've been training for 5 weeks, fatigue is 4/10, and performance is increasing."

**🤖 AI Agent:**
> Your status is Stable. No immediate deload is required at this time.

---

**👤 You:**
> "What exercises should I do during a hypertrophy phase deload?"

**🤖 AI Agent:**
> For a hypertrophy phase deload, focus on low volume with moderate intensity using stable movement variations.


## ❓ FAQ

**Q: What is a proactive deload?**
A proactive deload is a planned recovery period scheduled in advance to prevent injury and overtraining before performance drops.

**Q: How do I know if I need a reactive deload?**
You can use `evaluate_fatigue_status` to determine if your current fatigue levels and performance trends require an unscheduled recovery period.

**Q: Can I adjust my exercises during recovery?**
Yes, use `get_exercise_templates` to receive movement adjustment recommendations based on your current training phase.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/deload-week-planner](https://vinkius.com/en/ai-agent-connect/deload-week-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deload Week Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deload-week-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deload Week Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deload-week-planner": {
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
