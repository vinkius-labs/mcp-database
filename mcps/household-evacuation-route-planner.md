# Household Evacuation Route Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-evacuation-route-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-preparedness](../categories/emergency-preparedness.md)

Create actionable family departure plans, meeting point cards, and role assignments for emergency preparedness.

## Description
This MCP server helps households prepare for emergencies by synthesizing exits, mobility needs, and official guidance into clear plans. Use `get_departure_plan` to map out exit routes, `generate_meeting_point_card` to create printable gathering instructions, `assign_household_roles` to distribute responsibilities, and `create_practice_schedule` to maintain readiness through regular drills.


## Available Tools (4)
- **assign_household_roles**: Distributes specific emergency tasks to household members
- **create_practice_schedule**: Proposes a recurring schedule for running evacuation drills
- **generate_meeting_point_card**: Creates a concise, printable reference for where the family should gather
- **get_departure_plan**: Generates a step-by-step exit strategy for the household


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Evacuation Route Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me create a departure plan. Our exits are the front door and the back sliding door. We have a wheelchair user, and we have a car available."

**🤖 AI Agent:**
> Your primary route is through the front door to ensure the most direct path for the wheelchair. Your alternate route is the back sliding door. Please ensure the path to the front door is kept clear of obstacles at all times.

---

**👤 You:**
> "Assign roles for our family: Alice, Bob, and Charlie. The tasks are: Grab the emergency kit, Lead the group, and Assist the elderly."

**🤖 AI Agent:**
> Assignments: Alice is assigned to Lead the group, Bob is assigned to Grab the emergency kit, and Charlie is assigned to Assist the elderly.

---

**👤 You:**
> "Create a meeting point card. Our primary spot is the big oak tree in the front yard, and our secondary spot is the community center. We check in by calling the family group chat."

**🤖 AI Agent:**
> Meeting Point Card: Gather at the big oak tree in the front yard first. If that is unsafe, move to the community center. Once at a location, follow the check-in procedure: call the family group chat to confirm everyone is safe.


## ❓ FAQ

**Q: How do I create a departure plan?**
You can use the `get_departure_plan` tool by providing your available exits, any official guidance from local authorities, mobility needs, and transport options.

**Q: Can I assign specific tasks to family members?**
Yes, the `assign_household_roles` tool allows you to distribute specific responsibilities like Lead, Communicator, or Supply to each member of your household.

**Q: How often should we practice our evacuation?**
You can use `create_practice_schedule` to determine the next recommended drill date based on your preferred frequency, such as monthly or quarterly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-evacuation-route-planner](https://vinkius.com/en/ai-agent-connect/household-evacuation-route-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Evacuation Route Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-evacuation-route-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Evacuation Route Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-evacuation-route-planner": {
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
