# Family Care Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-care-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate caregiving tasks, helper availability, and complex coverage rules.

## Description
This MCP server provides a scheduling engine to coordinate caregiving tasks by reconciling recipient needs, helper availability, and coverage logic. Use `calculate_care_calendar` to generate complete schedules, `validate_helper_eligibility` to verify caregiver qualifications, `detect_scheduling_conflicts` to find overlaps or travel violations, and `generate_rotation_priority` to ensure fair task distribution among helpers.


## Available Tools (4)
- **calculate_care_calendar**: 
- **detect_scheduling_conflicts**: 
- **generate_rotation_priority**: 
- **validate_helper_eligibility**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Care Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a care calendar for these tasks: [{"name": "Medication", "start": "2024-07-04T08:00:00", "end": "2024-07-04T08:30:00", "skill": "Level_2"}] with these helpers: [{"name": "Alice", "availability": "08:00-12:00", "skill": "Level_2"}] and this recipient: [{"name": "Bob", "preferences": []}]"

**🤖 AI Agent:**
> The care calendar has been generated. Alice is assigned to the Medication task at 08:00 AM on July 4th, 2024.

---

**👤 You:**
> "Is Alice eligible for a High-Dependency task requiring Level_3 skill?"

**🤖 AI Agent:**
> No, Alice is not eligible because her skill level is Level_2 and the task requires Level_3.

---

**👤 You:**
> "Check for conflicts in these assignments: [{"task": "Task A", "helper": "Alice", "start": "10:00", "end": "11:00"}, {"task": "Task B", "helper": "Alice", "start": "11:15", "end": "12:00"}] with a 30 minute travel time."

**🤖 AI Agent:**
> A conflict was detected: the gap between Task A and Task B is only 15 minutes, which is less than the required 30 minute travel time.


## ❓ FAQ

**Q: How do I generate a full schedule?**
You can use the `calculate_care_calendar` tool by providing tasks, recipients, helpers, and appointments.

**Q: Can the tool check if a caregiver is qualified?**
Yes, the `validate_helper_eligibility` tool checks if a helper's skill level matches the task requirements and recipient preferences.

**Q: How are scheduling conflicts identified?**
The `detect_scheduling_conflicts` tool identifies time overlaps or violations of required travel time between tasks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-care-calendar](https://vinkius.com/en/ai-agent-connect/family-care-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Care Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-care-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Care Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-care-calendar": {
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
