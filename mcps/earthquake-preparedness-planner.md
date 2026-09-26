# Earthquake Preparedness Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/earthquake-preparedness-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-preparedness](../categories/emergency-preparedness.md)

Generate personalized household earthquake preparedness plans, supply assignments, and drill schedules.

## Description
This MCP server helps households prepare for seismic events by generating actionable documentation. Use `get_household_plan` to create a customized overview based on local guidance, `get_supplies_assignment` to distribute essential items based on mobility needs, `get_family_meeting_card` to establish communication protocols, and `get_practice_calendar` to schedule regular drills.


## Available Tools (4)
- **get_family_meeting_card**: Creates a concise communication card for family members to use during a separation event
- **get_household_plan**: Generates a comprehensive preparedness overview for the household
- **get_practice_calendar**: Generates a schedule for conducting preparedness drills
- **get_supplies_assignment**: Determines how supplies should be distributed among household members or stored


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Earthquake Preparedness Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a preparedness plan for a single-family house with two adults and one infant. Local guidance is 'Drop, Cover, and Hold On'."

**🤖 AI Agent:**
> Your household plan is ready. Based on your single-family house and the 'Drop, Cover, and Hold On' guidance, we recommend securing heavy furniture and keeping the infant's supplies in a central, accessible location.

---

**👤 You:**
> "How should I distribute my supplies? I have 2 adults and 1 elderly person with limited mobility. I have water, first aid, and flashlights."

**🤖 AI Agent:**
> Water and first aid kits should be placed in the immediate proximity of the elderly household member to ensure quick access during an event.

---

**👤 You:**
> "Generate a drill schedule for my family with monthly frequency."

**🤖 AI Agent:**
> Your monthly drill schedule includes: Month 1: Drop/Cover/Hold On drill; Month 2: Evacuation drill; Month 3: Supply check drill.


## ❓ FAQ

**Q: How does the tool handle local emergency instructions?**
The `get_household_plan` tool prioritizes the specific local guidance you provide above all other general advice to ensure compliance with local authorities.

**Q: Can I plan for family members with mobility issues?**
Yes. By including mobility needs in the household member list, `get_supplies_assignment` ensures essential items are placed near those who need them most, and `get_practice_calendar` includes accessibility drills.

**Q: What is included in the family meeting card?**
The `get_family_meeting_card` tool produces a structured card containing your primary and secondary meeting locations and a hierarchy of contact numbers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/earthquake-preparedness-planner](https://vinkius.com/en/ai-agent-connect/earthquake-preparedness-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Earthquake Preparedness Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `earthquake-preparedness-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Earthquake Preparedness Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "earthquake-preparedness-planner": {
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
