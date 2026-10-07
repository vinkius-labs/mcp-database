# Family Trip Schedule MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-trip-schedule)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build cohesive daily itineraries that balance biological needs with travel and activities.

## Description
This MCP server helps families plan balanced daily schedules. It uses biological anchors like nap windows and meal times to ensure children remain well-rested and fed, while integrating activities and travel segments. Use `generate_daily_itinerary` to create a full schedule, `validate_schedule_feasibility` to check if the plan is realistic for a child's age, `find_activity_gaps` to locate free time between naps, and `calculate_travel_impact` to understand how transit affects available activity time.


## Available Tools (4)
- **find_activity_gaps**: Identifies available time slots where activities can be inserted without disrupting biological anchors
- **generate_daily_itinerary**: Creates a complete chronological schedule for a single day based on provided constraints
- **validate_schedule_feasibility**: Checks if a proposed itinerary is realistic and sustainable for the family
- **calculate_travel_impact**: Calculates the total time lost to transit and the resulting impact on the available activity time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Trip Schedule** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a daily itinerary for a child who wakes up at 07:00, needs a nap from 13:00 to 15:00, and eats lunch at 12:00. Include a 60-minute museum visit."

**🤖 AI Agent:**
> 07:00 - Wake up
12:00 - Lunch
13:00 - Nap
15:00 - Museum Visit
16:00 - End of scheduled activities

---

**👤 You:**
> "Is this schedule feasible for a 12-month-old: 08:00 Wake, 10:00 Activity, 12:00 Meal, 13:00 Nap?"

**🤖 AI Agent:**
> The schedule is feasible with an energy score of 85.

---

**👤 You:**
> "How much time will I lose if I travel for 45 minutes between two activities?"

**🤖 AI Agent:**
> The total travel time is 45 minutes, reducing your available activity time by that amount.


## ❓ FAQ

**Q: How do I create a full day plan?**
You can use the `generate_daily_itinerary` tool by providing wake times, nap windows, meal times, and planned activities.

**Q: Can I check if my schedule is too tiring for my child?**
Yes, use `validate_schedule_feasibility` with the child's age to receive a feasibility report and energy score.

**Q: How do I find time for a new activity?**
Use `find_activity_gaps` to identify available time slots between your fixed biological anchors like naps and meals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-trip-schedule](https://vinkius.com/en/ai-agent-connect/family-trip-schedule)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Trip Schedule** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-trip-schedule` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Trip Schedule** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-trip-schedule": {
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
