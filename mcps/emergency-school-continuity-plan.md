# Emergency School Continuity Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emergency-school-continuity-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Synthesize school directives and household logistics into actionable continuity plans.

## Description
This MCP server acts as a decision-support engine for families facing school disruptions. It processes school directives, student schedules, and caregiver availability to generate four critical outputs: a chronological continuity calendar using `get_continuity_calendar`, a hardware readiness assessment via `get_equipment_plan`, specific adult-to-child assignments through `get_adult_assignments`, and a prioritized communication checklist with `get_communication_checklist`. It ensures that school guidance takes precedence and that no supervision gaps occur during transitions between in-person and remote learning.


## Available Tools (4)
- **get_equipment_plan**: Evaluates if the household has the necessary hardware and connectivity to support the current continuity state
- **get_adult_assignments**: Determines which adults are responsible for which children during specific time windows
- **get_communication_checklist**: Generates a list of necessary actions to notify school, caregivers, and pickup contacts
- **get_continuity_calendar**: Generates a chronological schedule of what each child should be doing, based on school directives and caregiver availability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency School Continuity Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The school just announced remote learning for tomorrow. Here are our schedules and caregiver availability: [JSON data]"

**🤖 AI Agent:**
> I have generated your continuity plan. Your children will transition to remote learning tomorrow. The continuity calendar shows a supervised block from 9:00 AM to 12:00 PM with Sarah, and the equipment plan confirms you have sufficient bandwidth for both students.

---

**👤 You:**
> "Check if we have enough devices for everyone to learn remotely."

**🤖 AI Agent:**
> The equipment plan indicates a Critical Shortage. You have two students requiring devices but only one functional laptop available in your inventory.

---

**👤 You:**
> "Who is responsible for watching the kids during the school closure tomorrow?"

**🤖 AI Agent:**
> Based on the caregiver availability, Mark is assigned to supervise Leo from 8:00 AM to 12:00 PM, and Elena is assigned to supervise Maya during the same window.


## ❓ FAQ

**Q: How does the tool handle conflicting school instructions?**
The engine applies school guidance precedence, meaning official school directives always override existing student schedules and parental preferences.

**Q: Can I use this to check if my internet is sufficient for remote learning?**
Yes, the `get_equipment_plan` tool evaluates your connectivity status against the requirements of all active learners to determine if your household is ready.

**Q: What happens if there is a gap in caregiver availability?**
The `get_continuity_calendar` tool will detect gaps where no caregiver is available during a required learning block and return an error to alert you.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emergency-school-continuity-plan](https://vinkius.com/en/ai-agent-connect/emergency-school-continuity-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency School Continuity Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-school-continuity-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency School Continuity Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-school-continuity-plan": {
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
