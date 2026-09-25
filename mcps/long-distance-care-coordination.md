# Long-Distance Care Coordination MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/long-distance-care-coordination)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate care for distant loved ones by synchronizing local support, remote assistance, and travel plans.

## Description
This MCP server provides a complete toolkit for managing care for individuals in different locations. It allows AI agents to build unified schedules using `generate_coordination_calendar`, organize support hierarchies with `build_support_roster`, manage travel budgets via `calculate_travel_logistics`, and establish communication cadences with `create_communication_workflow`. The system enforces local-first response rules and ensures remote check-ins respect the recipient's time zone.


## Available Tools (4)
- **calculate_travel_logistics**: Determines the feasibility and details of physical visits
- **build_support_roster**: Organizes contacts into a functional hierarchy for response planning
- **create_communication_workflow**: Establishes the cadence and methods for keeping the care circle informed
- **generate_coordination_calendar**: Creates a unified schedule of all care-related activities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Long-Distance Care Coordination** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a schedule for next week's visits and remote check-ins for a recipient in New York."

**🤖 AI Agent:**
> The coordination calendar for next week in New York includes a physical visit on Tuesday at 2:00 PM and remote check-ins on Wednesday and Friday at 10:00 AM.

---

**👤 You:**
> "Organize my contacts into a support roster."

**🤖 AI Agent:**
> The support roster has been organized: John (Local Tier) is the primary responder, while Sarah (Remote Tier) will provide digital oversight.

---

**👤 You:**
> "Check if a trip from London to Tokyo on June 1st is feasible with a $2000 budget."

**🤖 AI Agent:**
> The travel plan for June 1st is not feasible as the estimated cost is $2500, which exceeds your $2000 budget.


## ❓ FAQ

**Q: How does the system handle emergencies?**
The system follows a Local-First Response rule, prioritizing the local support roster for immediate needs before escalating to remote helpers.

**Q: Can I manage travel costs for visiting family?**
Yes, you can use `calculate_travel_logistics` to determine if planned visits fit within your specified budget.

**Q: How are remote check-ins scheduled?**
The `generate_coordination_calendar` tool ensures remote check-ins are scheduled within the recipient's waking hours based on their local time zone.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/long-distance-care-coordination](https://vinkius.com/en/ai-agent-connect/long-distance-care-coordination)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Long-Distance Care Coordination** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `long-distance-care-coordination` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Long-Distance Care Coordination** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "long-distance-care-coordination": {
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
