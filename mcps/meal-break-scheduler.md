# Meal Break Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/meal-break-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimizes meal and snack placement within a workday while respecting meeting conflicts and travel time.

## Description
The Meal Break Scheduler is an automated engine designed to organize your eating schedule. It identifies viable time windows using `calculate_available_slots` and places meals or snacks into your workday using `schedule_eating_events`. The engine accounts for meeting conflicts, required meal durations, and necessary commute time to ensure your breaks are feasible. You can also use `validate_schedule_compliance` to audit a proposed schedule and `get_spacing_efficiency` to see how well your breaks align with your preferred physiological spacing.


## Available Tools (4)
- **get_spacing_efficiency**: Events must include preferredGapAfter.

Calculates how well the current schedule adheres to the user's preferred spacing
- **schedule_eating_events**: Use JSON strings for arrays.

Places a list of meals and snacks into the workday respecting constraints
- **validate_schedule_compliance**: Audits a proposed schedule against hard constraints like meeting conflicts and commute time
- **calculate_available_slots**: Identifies all viable windows of time within a workday where a break could potentially occur


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meal Break Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you schedule my breakfast and lunch for a workday from 09:00 to 17:00 with a meeting at 12:00-13:00 and 15 minutes of commute?"

**🤖 AI Agent:**
> I have scheduled your breakfast at 08:30 and your lunch at 14:00, ensuring they do not conflict with your 12:00 meeting and allow for your 15-minute commute.

---

**👤 You:**
> "How efficient is my current schedule based on my preferred spacing?"

**🤖 AI Agent:**
> Your current schedule has an efficiency score of 95%, with only a 5-minute deviation from your preferred spacing.

---

**👤 You:**
> "Find available time slots in my workday between 08:00 and 18:00 with a meeting from 10:00 to 11:00."

**🤖 AI Agent:**
> The available time slots are 08:00 to 10:00 and 11:00 to 18:00.


## ❓ FAQ

**Q: How does the scheduler handle meeting conflicts?**
The engine ensures that no meal or snack overlaps with your fixed meeting blocks, treating them as hard constraints.

**Q: Does it account for travel time?**
Yes, the `schedule_eating_events` tool incorporates the specified commute minutes to ensure you have enough time to travel to and from your meal location.

**Q: Can I check if my manual schedule is valid?**
Yes, you can use the `validate_schedule_compliance` tool to check if a proposed schedule respects all constraints like meeting blocks and commute requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/meal-break-scheduler](https://vinkius.com/en/ai-agent-connect/meal-break-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meal Break Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meal-break-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meal Break Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meal-break-scheduler": {
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
