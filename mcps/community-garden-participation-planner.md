# Community Garden Participation Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/community-garden-participation-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Automate garden schedules, duty rotations, and member signup actions.

## Description
This MCP server transforms individual availability and preferences into a structured, fair, and automated community garden participation schedule. It manages the complexities of shared-duty rotations, ensuring communal responsibilities like tool cleaning and compost turning are distributed evenly. Use `generate_participation_calendar` to create schedules that respect travel constraints and availability, `identify_signup_actions` to manage administrative checklists, `map_supply_responsibilities` to assign tool maintenance, and `create_communication_plan` to coordinate member notifications.


## Available Tools (4)
- **create_communication_plan**: Defines the cadence and method of contact for garden-wide updates and individual session reminders
- **generate_participation_calendar**: Creates a full schedule of individual plot work and shared communal duties
- **identify_signup_actions**: Generates a checklist of administrative tasks a member must complete
- **map_supply_responsibilities**: Assigns specific tools or supplies to members based on the rotation schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Community Garden Participation Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a participation calendar for our garden members."

**🤖 AI Agent:**
> The participation calendar has been generated. Members are scheduled for weeding on Saturday and compost turning on Tuesday, with all travel constraints respected.

---

**👤 You:**
> "What tools do members need to bring for the next session?"

**🤖 AI Agent:**
> Based on the supply responsibility plan, John is responsible for the shovels and Sarah is responsible for the watering cans for this session.

---

**👤 You:**
> "Check if a new member is ready to participate."

**🤖 AI Agent:**
> The member is eligible to participate once the pending membership fee of $25 is paid.


## ❓ FAQ

**Q: How does the tool handle member availability?**
The `generate_participation_calendar` tool processes member preferences and travel constraints to ensure no one is assigned a session they cannot attend.

**Q: Can I assign tool maintenance tasks?**
Yes, use `map_supply_responsibilities` to assign specific tools to members based on the rotation schedule and their presence in the calendar.

**Q: How are new members onboarded?**
The `identify_signup_actions` tool generates a checklist of required administrative tasks, such as paying membership fees or completing registration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/community-garden-participation-planner](https://vinkius.com/en/ai-agent-connect/community-garden-participation-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Community Garden Participation Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `community-garden-participation-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Community Garden Participation Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "community-garden-participation-planner": {
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
