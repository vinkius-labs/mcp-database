# Shelter-in-Place Household Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shelter-in-place-household-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-preparedness](../categories/emergency-preparedness.md)

Create actionable emergency readiness plans by converting home layouts and official guidance into structured shelter strategies.

## Description
This MCP server provides a structured framework for emergency preparedness. It allows AI agents to transform home layouts, household member needs, and official local guidance into concrete, actionable plans. Using tools like `generate_shelter_plan`, `validate_room_safety`, `optimize_supply_placement`, and `audit_household_communication`, the agent can determine the safest rooms, optimize where to place life-sustaining supplies, and ensure communication protocols are robust for every household member.


## Available Tools (4)
- **audit_household_communication**: Verifies that the communication plan is robust enough to handle the specific household composition
- **generate_shelter_plan**: Generates the core actionable components of the emergency plan based on user inputs and guidance
- **optimize_supply_placement**: Determines the most logical and safe locations for supplies within the household
- **validate_room_safety**: Evaluates a specific room's suitability based on the provided home layout and safety requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shelter-in-Place Household Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a shelter-in-place plan for my family of three (two adults, one infant) in a two-story house with a basement, following local guidance to stay in an interior room."

**🤖 AI Agent:**
> Your primary shelter location is the interior hallway on the ground floor. You should move all supplies, including infant care items, to this location. Ensure the door is sealed and stay tuned to your battery radio.

---

**👤 You:**
> "Is the living room safe for sheltering if the official guidance requires an interior room with no windows?"

**🤖 AI Agent:**
> No, the living room is not safe because it contains windows, which violates the requirement for an interior room.

---

**👤 You:**
> "Where should I put my water bottles and first aid kit for the shelter plan?"

**🤖 AI Agent:**
> The water bottles and first aid kit should be placed in the designated safe room on the ground floor to ensure they are immediately accessible during the emergency.


## ❓ FAQ

**Q: How does the tool handle conflicting information?**
The tool follows a strict guidance precedence rule where official instructions from local authorities always override personal preferences or general best practices.

**Q: Can I use this to plan for family members with specific needs?**
Yes, the `generate_shelter_plan` tool evaluates the specific medical or mobility needs of all household members to ensure the selected room and supply placement are appropriate.

**Q: What information is required to generate a plan?**
You must provide the home layout, household member details, official local guidance, available supplies, communication options, and a list of accessible rooms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shelter-in-place-household-planner](https://vinkius.com/en/ai-agent-connect/shelter-in-place-household-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shelter-in-Place Household Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shelter-in-place-household-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shelter-in-Place Household Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shelter-in-place-household-planner": {
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
