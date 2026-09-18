# Intermittent Fasting Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/intermittent-fasting-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates personalized fasting schedules, meal timings, and adaptation forecasts.

## Description
This MCP server provides a specialized planning engine for intermittent fasting. It uses `generate_fasting_schedule` to create complete daily roadmaps, including eating windows and calorie distribution. Users can check protocol compatibility with `analyze_protocol_feasibility`, optimize meal times with `calculate_meal_timing`, and predict physiological adjustment periods using `get_adaptation_forecast`. The engine automatically accounts for medication schedules and exercise timing to ensure metabolic goals are met without health conflicts.


## Available Tools (4)
- **analyze_protocol_feasibility**: Evaluates if a specific protocol is compatible with a user's existing constraints
- **calculate_meal_timing**: Provides specific timing suggestions for meals within an established eating window
- **generate_fasting_schedule**: Creates a complete daily fasting and eating roadmap
- **get_adaptation_forecast**: Predicts the physiological adjustment period for a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Intermittent Fasting Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 16:8 fasting schedule for me. I wake up at 07:00 and I need to take medication at 09:00 and 19:00."

**🤖 AI Agent:**
> Your 16:8 fasting schedule is set. Your eating window is from 08:00 to 16:00. However, since you need medication at 19:00, your eating window has been shifted to 11:00 to 19:00 to accommodate your needs.

---

**👤 You:**
> "Is the OMAD protocol feasible if I exercise at 17:00 and take medicine at 08:00?"

**🤖 AI Agent:**
> No, the OMAD protocol is not feasible with your current constraints because your medication time at 08:00 falls outside the single meal window required for OMAD.

---

**👤 You:**
> "Suggest meal times for a 16:8 window starting at 12:00 with 3 meals."

**🤖 AI Agent:**
> For your 12:00 to 20:00 eating window, your recommended meal times are 12:00, 15:30, and 19:00.


## ❓ FAQ

**Q: How does the scheduler handle my medication?**
The `generate_fasting_schedule` tool automatically adjusts your eating window to ensure all medication times are included within the period when food is permitted.

**Q: Can I check if a protocol like OMAD is right for me?**
Yes, you can use `analyze_protocol_feasibility` to evaluate if a specific protocol is compatible with your existing constraints like medication or exercise.

**Q: How long will it take to adjust to a new fasting routine?**
You can use `get_adaptation_forecast` to receive a prediction of the physiological adjustment period based on your current dietary patterns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/intermittent-fasting-scheduler](https://vinkius.com/en/ai-agent-connect/intermittent-fasting-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Intermittent Fasting Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `intermittent-fasting-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Intermittent Fasting Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "intermittent-fasting-scheduler": {
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
