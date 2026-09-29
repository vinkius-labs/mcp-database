# Repair Downtime Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-downtime-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Schedules maintenance windows by coordinating repair durations, dependencies, and alternatives.

## Description
This MCP server provides a specialized scheduling engine to optimize maintenance windows. It coordinates repair durations, item dependencies, and temporary alternatives to ensure operational continuity. By analyzing user priorities and booking dates, it uses `calculate_continuity_strategy` to determine the best sequence of actions and `generate_downtime_plan` to produce a finalized schedule with assigned owners. It is designed to manage complex maintenance workflows for critical infrastructure.


## Available Tools (4)
- **calculate_continuity_strategy**: Determines the optimal sequence of actions by balancing repair needs against user priorities and the availability of alternatives
- **check_availability**: Validates if a proposed set of repair actions can fit within the user-defined booking dates
- **generate_downtime_plan**: Produces the final, formatted schedule including ownership assignments
- **get_repair_requirements**: Retrieves the technical requirements and dependency tree for a specific item needing repair


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Downtime Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a downtime plan for the Main Power Grid and Cooling Unit with the assigned owners."

**🤖 AI Agent:**
> 1. 08:00 - 10:00: Repair Main Power Grid (Owner: Electrical Team)
2. 10:00 - 11:00: Repair Cooling Unit (Owner: HVAC Team)

---

**👤 You:**
> "Check if these repair tasks fit within a 5-hour window."

**🤖 AI Agent:**
> The requested repair tasks cannot fit within the 5-hour window due to a dependency violation.

---

**👤 You:**
> "What are the requirements for the Primary Server?"

**🤖 AI Agent:**
> The Primary Server requires a 4-hour repair duration and depends on the Main Power Grid being operational.


## ❓ FAQ

**Q: How does the tool handle item dependencies?**
The engine respects the dependency tree. It ensures that prerequisite repairs are completed before dependent items begin their maintenance window.

**Q: Can I use temporary alternatives during repairs?**
Yes, the continuity strategy accounts for setup and teardown durations of alternatives to mitigate downtime impact.

**Q: How are conflicts resolved?**
Conflicts are resolved using user-defined priority values, ensuring high-priority items are addressed first.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-downtime-planner](https://vinkius.com/en/ai-agent-connect/repair-downtime-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Downtime Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-downtime-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Downtime Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-downtime-planner": {
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
